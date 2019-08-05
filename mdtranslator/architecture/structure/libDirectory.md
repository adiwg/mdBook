# mdTranslator

## Directory Structure

### /lib Directory

__/lib__ holds all scripts for the mdTranslator gem:
 
* __adiwg-mdtranslator.rb__ - specifies the environment for the "adiwg-mdtranslator" gem. 

* __/adiwg__ - holds all scripts for mdTranslator readers and writers.

![lib Directory](/assets/mdTranslator/dir_lib.png){caption}

### /lib/adiwg Directory

__/adiwg__ directory holds all scripts for mdTranslator readers and writers:

* __mdtranslator.rb__ - entry point for the adiwg-mdtranslator gem.

* __mdtranslator_cli.rb__ - entry point and code for the CLI.

* __/mdtranslator__ - directory holds all scripts for mdTranslator readers and writers.

![adiwg Directory](/assets/mdTranslator/dir_lib_adiwg.png){caption}

### /lib/adiwg/mdtranslator Directory

__/mdtranslator__ - directory holds all scripts for mdTranslator readers and writers:

* __version.rb__ - keeps the version number for mdTranslator code and a history of changes.

* __/internal__ - holds methods used across multiple readers and writers.

* __/readers__ - holds the code for all mdTranslator readers.

* __/writers__ - holds the code for all mdTranslator writers.

![mdtranslator Directory](/assets/mdTranslator/dir_lib_adiwg_mdtranslator.png){caption}

### /lib/adiwg/mdtranslator/internal Directory

__/internal__ - holds methods used across multiple readers and writers.

* __internal_metadata_obj.md__ - a collection of methods that construct objects that couple together to dynamically create the mdTranslator's internal data store.

* __module_codeListFun.md__ - a method to search a codelist for valid items.

* __module_coordinates.md__ - a collection of methods to convert lists of coordinates between strings and array in formats for ISO, FGDC, and GeoJSON.  Includes a method for computing bounding box coordinates from a GeoJSON Feature Collection. 

* __module_dateTimeFun.md__ - a collection of methods to handle date and time formats in ISO and string representations.

![internal Directory](/assets/mdTranslator/dir_lib_adiwg_mdtranslator_internal.png){caption}

### /lib/adiwg/mdtranslator/readers Directory

__/readers__ - holds all the code for mdTranslator readers.

* __mdReaders.rb__ - contains the method that accepts parameters from a call to mdTranslator and decides which reader to execute or to abort if a valid reader is not found.  If reader returns valid internal data store from the read, control is passed to mdWriters.rb if a writer was requested, otherwise returns read status to the user.

* __/{reader name}__ - holds all the code for a specific reader.  The directory name MUST be the code name of the reader. 

![readers Directory](/assets/mdTranslator/dir_lib_adiwg_mdtranslator_readers.png){caption}

### /lib/adiwg/mdtranslator/writers Directory

__/writers__ - holds all the code for mdTranslator writers.

* __mdWriters.rb__ - contains the method that accepts parameters from mdReaders.rb and decides which writer to execute or to abort if a valid writer is not found.  Returns results of the writer or error messages if writer execution fails.

* __/{writer name}__ - holds all the code for a specific writer.  The directory name MUST be the code name of the writer. 

![writers Directory](/assets/mdTranslator/dir_lib_adiwg_mdtranslator_writers.png){caption}
