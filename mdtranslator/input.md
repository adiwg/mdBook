# Architecture
## Input

As a rule, metadata input to the mdTranslator module is passed to the translator as a string variable in the parameter list invoking the translator.  However, when using the CLI a file name may substituted in place of the string.  The CLI interface will read the file into a string and then call mdTranslator in the usual way.

The translator does not examine the contents of the input metadata in any way.  This is left to the validation step next.  The translator simply looks for the name of the reader and asses the metadata string and other parameters to the reader.

If the requested reader cannot be found the translator will report back with the error.
