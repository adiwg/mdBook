# mdTranslator

## Extending the mdTranslator

### Creating Readers

New readers can be added with little to no impact on the base mdTranslator code. All code for a reader should be placed in folder structure with its root folder having the same name as given the reader.  The base mdTranslator code will transfer processing to the reader based on the name of the reader provided in the reader: parameter.  

A developer of a new reader should start by gaining an understanding of the [mdTranslator architecture](../mdtranslator/translatorArchitecture.md) and in particular the structure of the [internal object](../mdtranslator/internalObject.md) which the reader is responsible for loading properly so that all writers have access to the metadata content.

[__Reader Functions__](../mdtranslator/readerFunctions.md) - lists functions the reader is expected to perform on its own. 

[__Rules for Readers__](../mdtranslator/readerRules.md) - lists rules to follow when writing readers. 
