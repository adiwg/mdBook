#mdTranslator

## Usage

### Ruby

After installing the 'adiwg-mdtranlator' gem it can be accessed through a single exposed method - 'translate'.  Installation of the 'adiwg-mdtranslator' RubyGem was discussed in the section [Installation in Ruby](../mdtranslator/installInRuby.md) if that has not already be done.   

mdTranslator 'translate' method:
````ruby
module ADIWG
    module Mdtranslator

        def self.translate(file:, reader:, validate: 'normal', writer: nil, showAllTags: false)
````
The Ruby Gem adiwg-mdTranslator exposes the translate function as ADIWG::Mdtranslate.translate().  The parameters are entered as keyword parameters which requires Ruby 2.1.0 or higher. 

The translate method takes the following parameters:

__file:__ *string* (required) - accepts the contents of the input metadata file.  The file: string will be reade and interpreted by the reader specified in the reader parameter. 

__reader:__ *string* (required) - Provides the name of the desired reader to mdTranslator. This is the reader which will load, validate, and parse the input metadata into the *internal object*.  If the requested reader cannot be found by the translator, mdTranslator will report back with the error.

__validate:__ *string* ['none' | '**normal**' | 'strict'] (optional) - The validate parameter set the level of validation to be performed by the reader.  This is a function provided by the reader and is the specific actions are dependent on the input file format. The generic validation levels are:

* none - no validation
* normal - basic validation service (default)
* strict - check everything

Note that strict validation will likely cause your input file to fail pointing to deviations from the full standard that you did intended to make and will not actually cause the reader to fail.

__writer:__ *string* (optional) - Provides a writer name to mdTranslator.  If no writer is provided, processing will stop after the input metadata file has been validated and parsed into the *internal object*.

__showAllTags:__ *Boolean* (optional) - The action taken will be dependent on the metadata standard being written.  For example if the metadata standard is writing XML, empty or missing elements can either be eliminated from the output or shown as empty XML tags (e.g. < /myTag\>).

The mdTranslator [response hash](../mdtranslator/responseHash.md) is always returned by mdTranslator.translate even when the reader or writer fails to complete.  

Example call to mdTranslator translate:
````ruby
# returns 'response hash' object
metadata = ADIWG::Mdtranslator.translate(
    file: jsonObj, reader: 'mdJson', validate: 'normal',
    writer: 'iso19115_2', showAllTags: true)
````




