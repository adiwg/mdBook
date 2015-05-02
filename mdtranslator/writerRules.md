# mdTranslator

## Extending the mdTranslator

### Rules for Writers

New Writers should be added with little to no impact to the base mdTranslator code as changes to this code may impact existing Readers and Writers.  

Rules for creating a mdTranslator Writers: 

1. The Writer name {writer} should be not be same as another Writer name.
2. All Writer code will be contained within a folder structure with its root folder being the name of the Writer.  
3. The Writer's root folder will be placed within the mdtranslator/lib/adiwg/mdtranslator/writers/ folder.
4. All Writer files will be namespaced with ADIWG::Mdtranslator::Writers::{writer}.
5. The Writer's entry point will be a method 'startWriter(internalObj)'.  The internalObj object is the *metadata content hash* prepared by the Reader. 
6. The startWriter(internalObj) method will be in a Ruby file named '{writer}_writer.rb' in the Writer's root folder. 
7. A readme.md file will be in the Writer's root folder.  The file will be formatted in Markdown and used by [mdTranslator API](http://mdtranslator.adiwg.org/) website to identify the Writer. 

````ruby
module ADIWG
    module Mdtranslator
        module Writers
            module {writer}

                def self.startWriter(internalObject)
                    ...
````

The Writer must also be added to the [mdTranslator API](http://mdtranslator.adiwg.org/).  The code for mdTranslator website is kept in the [mdTranslator-rails](https://github.com/adiwg/mdTranslator-rails) repository.  

.1. Add the Writer name to the options list (mdtranslatorRails/app/modelsoption.rb)

````ruby
class Option
	def self.getOptionList
		hOptions = {
			readers: %w[mdJson],
			writers: %w[iso19115_2 iso19110 html {new writer}],
````
.2. Add a link to the new Writer's web page.  The page will be dynamically built by the Rails application.  It's content will be the content of the readme.md file placed in the Writer's root folder (see step 7 above). Below is the example for Writer iso19115_2.

````md
 [mdJson](./writers/iso19115_2)

 : International Standards Organization Geographic Information - Metadata 19115-2:2009
````
.3. mdTranslator-rails handles response types for metadata files generated in XML, JSON, HTML, and plain text.  If you are preparing metadata output in another format the translators_controller.rb will need to be extened to handle the new file type.   (mdtranslatorRails/app/controllers/api/v1/translators_controller.rb)


