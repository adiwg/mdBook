# mdTranslator

## Extending the mdTranslator

### Reader Functions

A reader receives a global [response hash](../mdtranslator/responseHash.md) from the mdTranslator.  The hash is used to communication status and pass messages to the user.  The Reader will populate the response hash as it performs its functions.

An mdTranslator Reader performs these function: 
1. Set the $response[:readerFormat] to the anticipated format of the input file.  
2. Determine if the input file received is in the anticipated format and syntactically correct so that its content can be accurately read. Set $response[:readerStructurePass] to true or false.
3. If the input file failed to pass its structural tests add one or more messages to the $response[:readerStructureMessages] array to help the user correct the problems.  
4. If the Reader name and version are imbeded in content file check these match values expected by the Reader.  Set $response[:readerFound] and $response[:readerVersionFound] to the values found in the input file. 
5. Set $response[:readerVersionUsed] to the actual version of the reader used to process the input file. 
6. The reader should validate the schema of the input file.  The validation should check that all required fields are populated, numbers are in numeric fileds, dates are valid, etc.  The mdTranslator parameter 'validate:' can be checked in $response[:readerValidationLevel] to determine level of validation the user has requested of the Reader.  It is left to the Reader to deterine the implications of the validation level.  Set $response[:readerValidationPass] to true or false depending on the outcome of the schema validation. 
7. If the schema validation failed add one or more messages to the $response[:readerValidationMessages] array to help the user correct any problems.
8. The reader should next unload the input file and build a *metadata content hash* in the structure defined by the [internal object](../mdtranslator/internalObject.md). The Reader must begin this process by creating an instance of the internal object's 'base object'.  The Reader should then instance other objects as defined by the *internal object* as they are needed to build up the metadata content hash. 
9. Set the $response[:readerExecutionPass] to true or false depending on the success of building the metadata content hash.
10. If errors or processing problems were encountered while the building the metadata content hash add one or more messages to the $response[:readerExecutionMessages] array.

All mdTranslator writers will use metadata content hash as their source data.  
