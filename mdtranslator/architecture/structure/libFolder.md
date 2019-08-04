# mdTranslator

## Directory Structure

### lib Directory

The "lib" folder has one file that specifies the environment for the "adiwg-mdtranslator" gem. 

![Project Directory](/assets/mdTranslator/dir_lib.png){caption}


### adiwg Folder

The "adiwg" folder has two files:
* "mdtranslator.rb" - entry point for the adiwg-mdtranslator gem
* "mdtranslator_cli.rb" - entry point and code for the CLI

![Project Directory](/assets/mdTranslator/dir_lib_adiwg.png){caption}

### mdtranslator Folder

The "mdtranslator" folder has one file that holds the version number for mdTranslator.

![Project Directory](/assets/mdTranslator/dir_lib_adiwg_mdtranslator.png){caption}

### internal Folder

The "internal" folder holds methods that are used across multiple readers and writers.

* "__internal_metadata_obj.md__" - a collection of methods that construct objects that couple together to dynamically create the mdTranslator's internal data store.

* "__module_codeListFun.md__" - a method to search a codelist for valid items.

* "__module_coordinates.md__" - a collection of methods to convert lists of coordinates between strings and array in formats for ISO, FGDC, and GeoJSON.  Includes a method for computing bounding box coordinates from a GeoJSON Feature Collection. 

* "__module_dateTimeFun.md__" - a collection of methods to handle date and time formats in ISO and string representations.

![Project Directory](/assets/mdTranslator/dir_lib_adiwg_mdtranslator_internal.png){caption}

### readers Folder

The "readers" folder holds the code for all mdTranslator readers.

### writers Folder

The "writers" folder holds the code for all mdTranslator writers.

