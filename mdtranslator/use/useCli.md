#mdTranslator

## Use CLI

 `$mdtranslator translate` provides command line access to the ADIwg metadata translator, mdTranslator. The "translate" method converts input metadata to supported established metadata metadata formats. The CLI accepts an input metadata file with options to select the input reader format, writer output format, display empty tags in XML outputs, and choose level of validation for mdJson input files.

*Usage*:
  mdtranslator translate [FILE] --reader=READER

*Options*:
  --reader=READER, -r
  > Name of input metadata file reader
  > Possible values: mdJson, fgdc, sbJson
  
  [--writer=WRITER], -w                    
  > Name of output metadata file writer
  > leave blank to validate input only  
  > Possible values: mdJson, iso19115-1, iso19115_2, iso19110, fgdc, html, sbJson  
  
  [--validate=VALIDATE], -v
  > Specify level of validation desired 
  > Default: normal   
  > Possible values: none, normal, strict
    
  [--showAllTags], [--no-showAllTags], -s    
  > Include tags for unused attributes
  
  [--messages=MESSAGES], -m                 
  > On error, return messages as formatted text or json object  
  > Default: text  
  > Possible values: json, text
                                             
  [--returnObject], [--no-returnObject], -o  
  > Return the full responseHash as a JSON object  
  
  [--cssLink=CSSLINK]                    
  > Provide a fully qualified link to a CSS file to overlay HTML writer CSS
  
  [--forceValid], [--no-forceValid], -f
  > Insert tags for required elements missing from input
  
#### CLI example

From terminal ...

````
$ mdtranslator translate "myFileName.json" --reader mdJson --writer iso19115_2
````
