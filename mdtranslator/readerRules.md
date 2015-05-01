# mdTranslator

## Extending the mdTranslator

### Rules for Readers

New Readers should be added with little to no impact to the base mdTranslator code as changes to this code may impact existing Readers and Writers.  

Rules for creating a mdTranslator Reader: 

1. The Reader name {reader} should be not be same as another Reader.
2. All Reader code will be contained within a folder structure with its root folder having the name of the Reader.  
3. The Reader's root folder will be placed within the mdtranslator/lib/adiwg/mdtranslator/readers/ folder.
4. All Reader files will be namespaced with ADIWG::Mdtranslator::Readers::{reader}.
5. The Reader's entry point will be a method readFile(file) in a Ruby file named '{reaer}_reader.rb'. 
6. A readme.md file will be in the root of Reader.  The file will be formatted in Markdown and used in the to identify the Reader in the [mdTranslator API](http://mdtranslator.adiwg.org/). 

````ruby
module ADIWG
    module Mdtranslator
        module Readers
            module {name}

                def self.readFile(file)
                    ...
````

The Reader must also be added to the [mdTranslator API](http://mdtranslator.adiwg.org/).

1. 