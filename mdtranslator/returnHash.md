# mdTranslator

## Architecture

### Response Hash


````ruby
# load and return this hash
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
