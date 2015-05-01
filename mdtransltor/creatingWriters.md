# mdTranslator

## Extending the mdTranslator

### Creating Writers

New Writers can be added with little to no impact on the base mdTranslator code. All code for a writer should be placed in folder structure with its root folder having the same name that was given to the writer.  The base mdTranslator code will transfer processing to the Writer based on the name of the Writer provided in the writer: parameter.  

A developer of a new reader should start by gaining an understanding of the [mdTranslator architecture](../mdtranslator/translatorArchitecture.md) and in particular the structure of the [internal object](../mdtranslator/internalObject.md) which the reader is responsible for loading properly so that all writers have access to the metadata content.

[__Reader Functions__](../mdtranslator/readerFunctions.md) - lists functions the reader is expected to perform on its own. 

[__Rules for Readers__](../mdtranslator/readerRules.md) - lists rules to follow when writing readers. 
