# mdTranslator

## Architecture

### Response Hash


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

__readerFormat:__ *string* - 

__readerStructurePass:__ *boolean* - 

__readerStructureMessages:__ *string[]* - an array of quoted string 

__readerRequested:__ *string* - 

__readerFound:__ *string* - 

__readerVersionFound:__ *string* - 

__readerVersionUsed:__ *string* - 

__readerValidationLevel:__ *string* - 

__readerValidationPass:__ *string* -

__readerValidationMessages:__ *string[]* - 

__readerExecutionPass:__ *boolean* - 

__readerExecutionMessages:__ *string[]* - 

__writerName:__ *string* - 

__writerVersion:__ *string* - 

__writerFormat:__ *string* - 

__writerPass:__ *boolean* - 

__writerMessages:__ *string[]* - 

__writerOutput:__ *string* - 


