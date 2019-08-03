# mdTranslator

### Command Line Interface 

The mdTranslator *command line interface* (CLI) is automatically installed with the 'adiwg-mdtranslator' RubyGem. It listens at the command line for any commands addressed to 'mdtranslator'.  Command line options allow specification of the input metadata file, reader, writer, and other mdTranslator parameters as listed below.  The CLI handles the interface with the mdTranslator.  It passes the file and options in, waits, and then catches the mdTranslator response and returns it to the user.  The mdTranslator result can be assigned to an application variable or piped to a file as required by the user.  The CLI output may be wrapped in JSON or XML or if desired the entire [responseHash](responseHash.md) can be returned. 

The Command Line Interface uses the RubyGem 'thor' to deliver its functionality.


The translate methods options are:

* __translate__ to connect with mdTranslator and request a metadata translation (see [Use CLI](../use/useCli.md) for details)

* __version__ to find version of installed mdTranslator CLI (automatically added by the thor gem).

* __help__ to display translate method options (automatically added by the thor gem).