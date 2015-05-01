# mdTranslator

## Extending the mdTranslator

### Writer Functions

A Writer receives a global [response hash](../mdtranslator/responseHash.md) from the mdTranslator.  The hash is used to communicate status and pass messages to the user.  The Writer will need to populate the response hash as it performs its functions.

An mdTranslator Writer performs these function: 
1. Set the $response[:writerFormat] to the format of the output metadata created by the Writer.
2. Set the $response[:writerVersion] to the version of the Writer creating the metadata output. 
2. Determine if the input file received is in the anticipated format and syntactically correct so that its content can be accurately read. Set $response[:readerStructurePass] to true or false.

An mdTranslator Writer formats the metadata content placed in the internal object by the Reader into a properly formatted metadata record.

Most content rules are associated with a metadata standard and vary greatly between standards.  For this reasons it is the responsibility of the Writer to decide how to handle missing or improperly formatted content found in the intern object. Each Writer may take a different approach to handling exceptions (e.g., in ISO 19115-2 a missing required element will set a tag attribue nilReason='missing'). In this scenario, the metadata record remains valid even with a required value missing.  
