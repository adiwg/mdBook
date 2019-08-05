# mdTranslator

## Extending the mdTranslator

### Creating Readers

New Readers can be added with little to no impact on the base mdTranslator code. All code for a reader should be placed in folder structure with its root folder having the same name that was given to the reader.  The base mdTranslator code will transfer processing to the Reader based on the name of the Reader provided in the reader: parameter.  

A developer of a new Reader should start by gaining an understanding of the [mdTranslator architecture](../mdtranslator/translatorArchitecture.md) and in particular the structure of the [internal object](../mdtranslator/internalObject.md) which the Reader is responsible for loading properly so that all writers have access to the metadata content.

[__Reader Functions__](../mdtranslator/readerFunctions.md) - a list of functions the Reader is expected to perform. 

[__Rules for Readers__](../mdtranslator/readerRules.md) - a list of rules for developing Readers. 

# mdTranslator

## Extending the mdTranslator

### Creating Writers

New Writers can be added with little to no impact on the base mdTranslator code. All code for a writer should be placed in folder structure with its root folder having the same name that was given to the writer.  The base mdTranslator code will transfer processing to the Writer based on the name of the Writer provided in the writer: parameter.  

A developer of a new Writer should start by gaining an understanding of the [mdTranslator architecture](../mdtranslator/translatorArchitecture.md) and in particular the structure of the [internal object](../mdtranslator/internalObject.md) from which the Writer will access the metadata content.

[__Writer Functions__](../mdtranslator/writerFunctions.md) - a list of functions the Writer is expected to perform. 

[__Rules for Writers__](../mdtranslator/writerRules.md) - a list of rules for developing Writers. 
