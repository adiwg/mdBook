# mdTranslator

## Extending the mdTranslator

New readers and writers can be added with little to no impact on the base mdTranslator code.  New readers and writers also should be written in a way that will not interfere with existing reades and writers.

A developer of a new reader of writer should start by gaining an understanding of the [mdTranslator architecture](../mdtranslator/translatorArchitecture.md) and in particular the structure of the [internal object](../mdtranslator/internalObject.md) which all readers will write to and all writers will read from.

And of course, a reasonable understanding of the Ruby development language is required. 

[__Creating Readers__](../mdtranslator/creatingReaders.md) - 

[__Creating Writers__](../mdtranslator/creatingWriters.md) - 
