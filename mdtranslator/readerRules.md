# mdTranslator

## Extending the mdTranslator

### Rules for Readers

New Readers should be added with little to no impact to the base mdTranslator code as changes to this code may impact existing Readers and Writers.  

Rules for creating a mdTranslator Reader: 

1. The Reader name {reader} should be not be same as another Reader name.
2. All Reader code will be contained within a folder structure with its root folder being the name of the Reader.  
3. The Reader's root folder will be placed within the mdtranslator/lib/adiwg/mdtranslator/readers/ folder.
4. All Reader files will be namespaced with ADIWG::Mdtranslator::Readers::{reader}.
5. The Reader's entry point will be a method 'readFile(file)'.
6. The readFile(file) method will be in a Ruby file named '{reaer}_reader.rb' in the Reader's root folder. 
7. A readme.md file will be in the Reader's root folder.  The file will be formatted in Markdown and used by [mdTranslator API](http://mdtranslator.adiwg.org/) website to identify the Reader. 

````ruby
module ADIWG
    module Mdtranslator
        module Readers
            module {name}

                def self.readFile(file)
                    ...
````

The Reader must also be added to the [mdTranslator API](http://mdtranslator.adiwg.org/).  The code for mdTranslator website is kept in the [mdTranslator-rails](https://github.com/adiwg/mdTranslator-rails) repository.  

.1. Add the Reader name to the options list (mdtranslatorRails/app/modelsoption.rb)

````ruby
class Option
	def self.getOptionList
		hOptions = {
			readers: %w[mdJson {new reader}],
			writers: %w[iso19115_2 iso19110 html],
````
.2. Add a ling to the new Reader's web page.  The page will be dynamically built by the Rails application.  It's content will be the content of the readme.md file placed in the Reader's root folder (see step 7 above). Below is the example for Reader mdJson.

````md
 [mdJson](./readers/mdJson)

 : Alaska Data Integration working group JSON metadata format
````
.3. mdTranslator-rails handles response types for metadata files generated in XML, JSON, HTML, and plain text.  If you are preparing metadata output in another format the translators_controller.rb will need to be extened to handle the new file type.   (mdtranslatorRails/app/controllers/api/v1/translators_controller.rb)
