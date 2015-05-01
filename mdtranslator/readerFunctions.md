# mdTranslator

## Extending the mdTranslator

### Reader Functions

New readers can be added with little to no impact on the base mdTranslator code. All code for a reader should be placed in folder structure with its root folder having the same name as given the reader.  The base mdTranslator code will transfer processing to the reader based on the name of the reader provided in the reader: parameter.  

A developer of a new reader should start by gaining an understanding of the [mdTranslator architecture](../mdtranslator/translatorArchitecture.md) and in particular the structure of the [internal object](../mdtranslator/internalObject.md) which the reader is responsible for loading properly so that all writers have access to the metadata content.

[__Reader Functions__](../mdtranslator/readerFunctions.md) - lists functions the reader is expected to perform on its own. 

[__Rules for Readers__](../mdtranslator/readerRules.md) - lists rules to follow when writing readers. 
Reader Functions

# Reader Functions

An mdTranslator Reader performs two basic function: 1) to validate the input file meets the standards for the Reader specification; and 2) load the contents of the input file into the translator's internal object.

How these tasks are accomplished by a Reader are dependent on the format and organization of the input metadata file.  The next sections will discuss how the mdJson Reader embedded in mdTranslator meets these objectives.

## Validate

Validation of the input metadata file is one of two Reader responsibilities.  How a Reader performs this responsibility and what constitutes 'valid' is totally dependent on the file format and metadata standard of the input file.

As an example of what a Reader could do to determine the validity of an input file, we can look at the actions taken by the mdJson Reader which is imbedded in mdTranslator.

1. The input file is passed through a JSON parser to validate it meets the basic structure and syntax for any JSON file.  All discernable errors detected by the parser are reported back to the mdTranslator and forward on to the requestor.
2. If the basic JSON structure is valid, the Ruby Gem json-schema is used along with our schema definition for mdJson to test if the input file meets all the syntax requirements for mdJson metadata files.  The mdJson file is checked to see if elements are organized into their proper JSON sturctures, if element values have the proper datatype, and if all required elements are present.  Again, any discernable errors detected by json-schema are reported back to the mdTranslator and passed along to the requestor.

If the mdJson file passes the above tests the reader will load it into the mdTranslator's internal object.  See next section.

## Load Internal Object

Once an input metadata file is determined to be valid it can be read into the mdTranslator's internal object.  The internal object is a Ruby hash which uses keys as symbols rather than the implicit form which uses strings as keys.

````ruby
schema = { name: 'mdJson', version: '1.0.1' }
schema[:name] #=> mdJson
````

All mdTranslator writers will access their metadata content from this hash.  See the [Internal Object](Internal Object) section for information on the structure of the internal hash.
