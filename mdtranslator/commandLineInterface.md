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

The mdTranslator translate options are:





