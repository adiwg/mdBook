#mdTranslator

## Use CLI

 `$mdtranslator translate` provides command line access to the ADIwg metadata translator, mdTranslator. The "translate" method converts input metadata to supported established metadata metadata formats. The CLI accepts an input metadata file with options to select the input reader format, writer output format, display empty tags in XML outputs, and choose level of validation for mdJson input files.

From terminal type...

````
mdtranslator translate "[FileName]" --reader [readerName] --writer [writerName]
````

example:

````
$ mdtranslator translate "myFileName.json" --reader mdJson --writer iso19115_2
````

#### Methods:

* __translate__ - passes an input metadata file to mdTranslator and returns the result.
  ````
  $ mdtranslator translate ...
  ````

* __help__ - displays a list of all "translate" options in the terminal window.
  ````
  $ mdtranslator help translate 
  ````

* __version__ displays the version of mdTranslator in the terminal window.

  ````
  $ mdtranslator version 
  ````

#### Options:

* __file__ (required) - the metadata content organized in the format required by the metadata standard of the reader option.  The value of *file* is first checked to see if it is a valid file name in the users local file system. If it is a file name the CLI attempts to read the file's content.  If it is not a valid file name 'file' is assumed to be a string containing the metadata content. 

* __--reader__ (alias -r, default mdJson) - name of the reader to read the file's content [__mdJson__ | fgdc | sbJson].

* __--writer__ (alias -w) - name of the writer to write the metadata content into a chosen standard. If not specified the input will be validated only [fgdc | html | iso19110 | iso19115_1 | iso19115_2 | mdJson | sbJson].

* __--validate__ (alias -v, default normal) - specify the level of validation required [none | __normal__ | strict].

* __--forceValid__ (alias -f, default true)- Insert tags for required elements missing from input [__true__ | false].

* __--showAllTags__ (alias -s, default false) - include tags in the output for unused metadata attributes [true | __false__].  

* __--messages__ (alias -m, default text) - on error, return messages as * formatted text or JSON object [__text__ | json].

* __--cssLink__ provide a fully qualified link to a CSS file to customize HTML writer output.

* __--returnObject__ (alias -o, default false) - if "true" return the full [responseHash](responseHash.md) in a JSON object [true | __false__], otherwise only the output from the writer is returned.
