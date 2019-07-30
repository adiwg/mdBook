# Reader Functions
## Validate

Validation of the input metadata file is one of two Reader responsibilities.  How a Reader performs this responsibility and what constitutes 'valid' is totally dependent on the file format and metadata standard of the input file.

As an example of what a Reader could do to determine the validity of an input file, we can look at the actions taken by the mdJson Reader which is imbedded in mdTranslator.

1. The input file is passed through a JSON parser to validate it meets the basic structure and syntax for any JSON file.  All discernable errors detected by the parser are reported back to the mdTranslator and forward on to the requestor.
2. If the basic JSON structure is valid, the Ruby Gem json-schema is used along with our schema definition for mdJson to test if the input file meets all the syntax requirements for mdJson metadata files.  The mdJson file is checked to see if elements are organized into their proper JSON sturctures, if element values have the proper datatype, and if all required elements are present.  Again, any discernable errors detected by json-schema are reported back to the mdTranslator and passed along to the requestor.

If the mdJson file passes the above tests the reader will load it into the mdTranslator's internal object.  See next section.



