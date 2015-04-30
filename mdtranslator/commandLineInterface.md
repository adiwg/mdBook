# mdTranslator

## Architecture

### Command Line Interface 

The mdTranslator *command line interface* (CLI) is installed with the 'adiwg-mdtranslator' RubyGem. It listens at the command line for any commands addressed to 'mdtranslator'.  Command line options allow specification of the input metadata file, reader, writer, and other mdTranslator parameters.  The CLI handles the interface with the mdTranslator.  It passes the file and options in and catches the mdTranslator response and returns it to the user.  The mdTranslator result can be assigned to an applicationi variable or piped to a file as required by the user.  The CLI output may be wrapped in JSON or XML or if desired the entire [response hash](../mdtranslator/responsehash.rb) can be returned. 

The Command Line Interface uses the RubyGem 'thor' to deliver its functionality.

The mdTranslator CLI functions are:

__translate__ - passes an input metadata file to mdTranslator and returns the result 
````
$ mdtranslator translate ...
````

__version__ - returns the current version number of mdTranslator CLI
````
$ mdtranslator version 
````

The translate function options are:

__file__ (required) - the metadata content organized in the format specified by the reader option.  The value of *file* is first checked to see if it is a valid file name in the users local file system. If it is a file name the CLI attempts to read the file's content.  If it is not a valid file name 'file' is assumed to be a string containing the metadata content. 

__--reader__ (alias -r, defalut mdJson) - name of the reader to read the file's content.

__--writer__ (alias -w) - name of the writer to write the metadata content into a chosen standard. If not specified the input will be validated only.

__--validate__ (alias -v, default normal) - specify the level of validation required [none | __normal__ | strict]

__--showAllTags__ (alias -s, default false) - include tags in the output for unused metadata attributes.  

__--messages__ (alias -m, default text) - on error, return messages as formatted test ofr JSON object.

__--returnObject__ (alias -o, default false) - return the full [response hash](../mdtranslator/responsehash.rb) in a JSON object.
