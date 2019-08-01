# mdTranslator

## Extending the mdTranslator

New readers and writers can be added with little to no impact on the base mdTranslator code.  New readers and writers also should be written in a way that will not interfere with existing reades and writers.

A developer of a new reader or writer should start by gaining an understanding of the [mdTranslator architecture](../mdtranslator/translatorArchitecture.md) and in particular the structure of the [internal object](../mdtranslator/internalObject.md) which all readers will write to and all writers will read from.

And of course, a reasonable understanding of the Ruby development language is required. 

[__Fork the Reposotory__](forkRepository.md) - covers creating a personal copy fo the mdTranslator code library for your use or to develop extensions.

[__Creating Readers__](../mdtranslator/creatingReaders.md) - lists functions of the reader and rules to follow when writing them. 

[__Creating Writers__](../mdtranslator/creatingWriters.md) - lists functions of the writer and rules to follow when writing them. 
