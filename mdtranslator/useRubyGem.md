#mdTranslator

## Usage

### Ruby

After installing the 'adiwg-mdtranlator' gem it can be accessed through a single exposed method - 'translate'.  Installation of the 'adiwg-mdtranslator' RubyGem was discussed in the section [Installation in Ruby](../mdtranslator/installInRuby.md) if that has not already be done.   

Example call to translate:
````ruby
# returns 'response hash' object
metadata = ADIWG::Mdtranslator.translate(
    file: jsonObj, reader: 'mdJson', validate: 'normal',
    writer: 'iso19115_2', showAllTags: true)
````

The translate method uses a named parameter list so the order of parameters is not important. The translate method takes the following parameters:

__file:__ (required) - the metadata content organized in the format specified by the reader option.  The value of *file* is first checked to see if it is a valid file name in the users local file system. If it is a file name the CLI attempts to read the file's content.  If it is not a valid file name 'file' is assumed to be a string containing the metadata content. 

__reader:__ (required) - name of the reader to read the file's content.

__writer:__ - name of the writer to write the metadata content into a chosen standard. If not specified the input will be validated only.

__validate:__ (default normal) - specify the level of validation desired [none | __normal__ | strict]

__showAllTags:__ (default false) - include tags in the output for unused metadata attributes.  This option may not apply to all writers. 

The mdTranslator [response hash](../mdtranslator/responseHash.md) is always returned by mdTranslator.translate even when the reader or writer fail to complete.  