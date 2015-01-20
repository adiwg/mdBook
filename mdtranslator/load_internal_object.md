# Reader Functions
## Load Internal Object

Once an input metadata file is determined to be valid it can be read into the mdTranslator's internal object.  The internal object is a Ruby hash which all mdTranslator writers will access to get the metadata content.  See the [Internal Object](Internal Object) section for more information.  Loading the contents of the input file to the internal object rather than directly converting the content into a metadata standard allows the input file access to all the mdTranslator's writers.


