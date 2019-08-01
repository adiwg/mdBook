#mdTranslator

## Use as Ruby Gem

After installing the 'adiwg-mdtranlator' gem it can be accessed through a single exposed method - 'translate'.  Installation of the 'adiwg-mdtranslator' RubyGem is covered in the section [Installation in Ruby](/mdtranslator/install/installInRuby.md) if it has not already be installed.   

mdTranslator 'translate' method is defined in the "mdtranslator.rb" method:

````ruby
module ADIWG
   module Mdtranslator

      def self.translate(file:, reader: 'mdJson', writer: nil, validate: 'normal', forceValid: true,
         showAllTags: false, cssLink: nil)
         
         # ... code
         
      end 
   end 
end

````

The Ruby Gem adiwg-mdTranslator exposes the translate function as ADIWG::Mdtranslate.translate().  The parameters are entered as keyword parameters which requires Ruby 2.1.0 or higher. 

The translate method takes the following parameters:

__file:__ *string* (required) - accepts the contents of the input metadata file.  The file: string will be reade and interpreted by the reader specified in the reader parameter. 

__reader:__ *string* (optional default:'mdJson') - Provides the name of the desired reader to mdTranslator. This is the reader which will load, validate, and parse the input metadata into the *internal object*.  If the requested reader cannot be found by the translator, mdTranslator will report back with the error.

__writer:__ *string* (optional) - Provides a writer name to mdTranslator.  If no writer is provided, processing will stop after the input metadata file has been validated and parsed into the *internal object*.


__validate:__ *enumerated* ['none' | '**normal**' | 'strict'] (optional default: 'normal') - The validate parameter set the level of validation to be performed by the reader.  This is a function provided by the reader and is the specific actions are dependent on the input file format. The generic validation levels are:

* none - no validation
* normal - basic validation service (default)
* strict - check everything

  Note that strict validation will likely cause your input file to fail pointing to deviations from the full standard that you did intended to make and will not actually cause the reader to fail.

__forceValid:__ *Boolean* (optional default:true) Force the output to be valid to the metadata standard by adding tags for missing elements.  Tag values will set to 'missing' for FGDC and nilReason="missing" for ISO.  Missing objects cannot be handled and result in an ERROR flag being set for the writer.

__showAllTags:__ *Boolean* (optional default:false) - The action taken will be dependent on the metadata standard being written.  For example if the metadata standard is writing XML, empty or missing elements can either be eliminated from the output or shown as empty XML tags (e.g. < /myTag\>).

__cssLink:__ *string* - (optional) The fully qualified path and file name to a CSS file to overlay the build-in CSS.  

The mdTranslator [response hash](../mdtranslator/responseHash.md) is always returned by mdTranslator.translate even when the reader or writer fails to complete.  

Below is an example call to mdTranslator translate:

````ruby

# read mdJson file
    file = 'myFile.json'
    file = File.open(file, 'r')
    jsonFile = file.read
    file.close
    jsonObj = JSON.parse(jsonFile)
 
# returns 'response hash' object 
metadata = ADIWG::Mdtranslator.translate(
    file: jsonObj, reader: 'mdJson', validate: 'normal',
    writer: 'iso19115_2', showAllTags: true)
    
````