# Ruby Gem

## Calling the mdTranslator

###mdTranslator Parameters
````ruby
module ADIWG
    module Mdtranslator

        def self.translate(file:, reader:, validate: 'normal', writer: nil, showAllTags: false)
````
The Ruby Gem adiwg-mdTranslator exposes the translate function as ADIWG::Mdtranslate.translate().  The parameters are entered as keyword parameters which requires interpretations by Ruby 2.1.0 or higher.

**file:** *string* (required)

As a general rule, metadata is input to the translator module as a string parameter in the mdTranslator's parameter list.  The only exception is when calling *translate* from the command line, then a file name may substituted in place of the string.  The command line interface (CLI) will read the file into a string and then pass the file to mdTranslator in the usual way.

**reader:** *string* (required)

Provides the name of the desired reader to mdTranslator. This is the reader which will load, validate, and parse the input metadata into the *internal object*.  If the requested reader cannot be found by the translator, mdTranslator will report back with the error.

**validate:** *string* ['none' | '**normal**' | 'strict'] (optional)

The validate parameter set the level of validation to be performed by the reader.  This is a function provided by the reader and is the specific actions are dependent on the input file format. The generic validation levels are:

* none - no validation
* normal - basic validation service (default)
* strict - check everything

Note that strict validation will likely cause your input file to fail pointing to deviations from the full standard that you did intended to make and will not actually cause the reader to fail.

**writer:** *string* (optional)

Provides a writer name to mdTranslator.  If no writer is provided, processing will stop after the input metadata file has been validated and parsed into the *internal object*.

**showAllTags:** *Boolean* (optional)

The action taken will be dependent on the metadata standard being written.  For example if the metadata standard is writing to XML, empty or missing elements can either be eliminated from the output or shown as empty XML tags (e.g. < /myTag\>).

