# mdTranslator

## Extending the mdTranslator

### Writer Functions

A Writer receives a global [response hash](../mdtranslator/responseHash.md) from the mdTranslator.  The hash is used to communicate status and pass messages to the user.  The Writer will need to populate the response hash as it performs its functions.

An mdTranslator Writer performs these function: 
1. Set the $response[:writerFormat] to the format of the output metadata record being created by the Writer.
2. Set the $response[:writerVersion] to the version of the Writer creating the metadata output record. 
3. Build the metadata output record in the standard implemented by the Writer.  The metadata content for the Writer is the *metadata content hash* returned from the Reader and passed to the Writer. 
3. Set the $response[:writerPass] to true or false depending on the success of building the metadata output record.
4. If errors or processing problems were encountered while building the metadata output record add one or more messages to the $response[:writerMessages] array to help the user correct the problems. 
5. Place the completed metadata output record in $response[:writerOutput] for distribution to the user. 


