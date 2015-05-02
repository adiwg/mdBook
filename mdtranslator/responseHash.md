# mdTranslator

## Architecture

### Response Hash

The *response hash* object is constructed by mdTranslator and available to reader and writer during its run. This is the object returned to the user at the completion of the run.  The reader and writer fill in object as they process the metadata content. 

````ruby
$response = {
    readerFormat: nil,
    readerStructurePass: nil,
    readerStructureMessages: [],
    readerRequested: reader,
    readerFound: nil,
    readerVersionFound: nil,
    readerVersionUsed: nil,
    readerValidationLevel: validate,
    readerValidationPass: nil,
    readerValidationMessages: [],
    readerExecutionPass: nil,
    readerExecutionMessages: [],
    writerName: writer,
    writerVersion: nil,
    writerFormat: nil,
    writerPass: nil,
    writerMessages: [],
    writerOutput: nil
}
````

__readerFormat:__ *string* - the anticipated format of the input file, parsing by the reader will proceed assuming this format.  Set by reader.

__readerStructurePass:__ *boolean* - 'true' if input file structure is determined to be valid.  Set by the reader.

__readerStructureMessages:__ *string[]* - an array of quoted string messages. If readerStructurePass is 'false', set one or more messages 
to assist the user in fixing file structure problems.  Set by reader. 

__readerRequested:__ *string* - name of the reader requested by the user. Set from the translate parameter list.

__readerFound:__ *string* - name of the reader used by the reader. Set by reader.  This will be same as readerRequested if the readerRequested name is valid. 

__readerVersionFound:__ *string* - version of the reader requested by the input file. Set by reader.

__readerVersionUsed:__ *string* - version of the reader the reader method decided to use in processing the input file.  Set by  reader.  Default 'normal'.

__readerValidationLevel:__ *string* - validation level requested to be applied to the input file.  Set from the parameter list.

__readerValidationPass:__ *string* - 'true' if the input file passes the level of validation requested.  Set by reader.

__readerValidationMessages:__ *string[]* - an array of quoted string messages. If readerValidationPass is 'false', set one or more messages to assist user fixing file schema validation problems.  Set by reader.

__readerExecutionPass:__ *boolean* - 'true' if the reader completes the import of the input file into the internal object without errors.  Set by the reader. 

__readerExecutionMessages:__ *string[]* - an array of quoted string messages. If readerExecutionPass is 'false', set one or more messages to assist user in fixing file data problems.  Set by reader.

__writerName:__ *string* - name of the writer requested by the user, set from the translate parameter list.  if nil, no write was requested and only validation of the input file will be performed.

__writerVersion:__ *string* - current version of the writer requested.  Set by writer.

__writerFormat:__ *string* - format of the output from the writer.  Set by writer.

__writerPass:__ *boolean* - 'true' if the writer completes the creation of the output file without errors.  Set by writer.

__writerMessages:__ *string[]* - an array of quoted string messages.  If writerPass is 'false', set one or more messages to assist user in fixing file data problems.  Set by writer.

__writerOutput:__ *string* - output file returned from the writer.  Set by writer.


