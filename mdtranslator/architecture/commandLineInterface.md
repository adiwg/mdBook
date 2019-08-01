# mdTranslator

### Command Line Interface 

The mdTranslator *command line interface* (CLI) is automatically installed along with the 'adiwg-mdtranslator' RubyGem. It listens at the command line for any commands addressed to 'mdtranslator'.  Command line options allow specification of the input metadata file, reader, writer, and other mdTranslator parameters as listed below.  The CLI handles the interface with the mdTranslator.  It passes the file and options in, waits, and then catches the mdTranslator response and returns it to the user.  The mdTranslator result can be assigned to an application variable or piped to a file as required by the user.  The CLI output may be wrapped in JSON or XML or if desired the entire [responseHash](responseHash.md) can be returned. 

The Command Line Interface uses the RubyGem 'thor' to deliver its functionality.

The mdTranslator CLI functions are:

__translate__ - passes an input metadata file to mdTranslator and returns the result 
````
$ mdtranslator translate ...
````

Help for the CLI is available through the help command
````
$ mdtranslator help translate 
````

The current version of the CLI is accessible via the __version__ command
````
$ mdtranslator version 
````

The translate method options are:

__file__ (required) - the metadata content organized in the format specified by the reader option.  The value of *file* is first checked to see if it is a valid file name in the users local file system. If it is a file name the CLI attempts to read the file's content.  If it is not a valid file name 'file' is assumed to be a string containing the metadata content. 

__--reader__ (alias -r, default mdJson) - name of the reader to read the file's content [__mdJson__ | fgdc | sbJson].

__--writer__ (alias -w) - name of the writer to write the metadata content into a chosen standard. If not specified the input will be validated only [fgdc | html | iso19110 | iso19115_1 | iso19115_2 | mdJson | sbJson].

__--validate__ (alias -v, default normal) - specify the level of validation required [none | __normal__ | strict].

__--forceValid__ (alias -f, default true)- Insert tags for required elements missing from input [__true__ | false].

__--showAllTags__ (alias -s, default false) - include tags in the output for unused metadata attributes [true | __false__].  

__--messages__ (alias -m, default text) - on error, return messages as formatted text or JSON object [__text__ | json].

__--cssLink__ provide a fully qualified link to a CSS file to customize HTML writer output.

__--returnObject__ (alias -o, default false) - if "true" return the full [responseHash](responseHash.md) in a JSON object [true | __false__], otherwise only the output from the writer is returned.
