# mdTranslator

### Response Hash

The *response hash* object is constructed by mdTranslator and available to reader and writer during its run. This is the object returned to the user at the completion of the run.  The reader and writer fill in object as they process the metadata content. 

````ruby
 hResponseObj = {
    readerRequested: nil,
    readerVersionRequested: nil,
    readerVersionUsed: nil,
    readerStructurePass: true,
    readerStructureMessages: [],
    readerValidationLevel: nil,
    readerValidationPass: true,
    readerValidationMessages: [],
    readerExecutionPass: true,
    readerExecutionMessages: [],
    writerRequested: nil,
    writerVersion: nil,
    writerPass: true,
    writerMessages: [],
    writerOutputFormat: nil,
    writerOutput: nil,
    writerForceValid: true,
    writerShowTags: false,
    writerCSSlink: nil,
    writerMissingIdCount: '_000',
    translatorVersion: nil
 }

````
         # the reader and writer specified in the translate module parameter string will load and
         #     return this hash ...
         # ====================================================================================
         # readerRequested: name of the reader requested by the user
         #   - set from the parameter list (reader) (default = 'mdJson')
         # ------------------------------------------------------------------------------------
         # readerVersionRequested: version of the reader requested in input file
         #   - set in reader
         # ------------------------------------------------------------------------------------
         # readerVersionUsed: actual reader version use in processing the input file
         #   - set by the reader
         # ------------------------------------------------------------------------------------
         # readerStructurePass: false if input file structure is determined to be invalid
         #   - set by the reader
         # ------------------------------------------------------------------------------------
         # readerStructureMessages: an array of parser warning and error messages
         #   - set by the reader
         # ------------------------------------------------------------------------------------
         # readerValidationLevel: validation level requested to be applied to the input file, set
         #   - set from the parameter list (reader)
         # ------------------------------------------------------------------------------------
         # readerValidationPass: false if fails requested level of validation
         #   - set by the reader
         # ------------------------------------------------------------------------------------
         # readerValidationMessages: an array of schema warning and error messages
         #   - set by the reader
         # ------------------------------------------------------------------------------------
         # readerExecutionPass: false if the reader finds fatal errors in input file
         #   - set by the reader
         # ------------------------------------------------------------------------------------
         # readerExecutionMessages: an array of reader warning and error messages
         #   - set by the reader
         # ------------------------------------------------------------------------------------
         # writerRequested: name of the writer requested by the user
         #   - set from the parameter list (writer)
         # ------------------------------------------------------------------------------------
         # writerVersion: version of the writer used within mdTranslator
         #   - set by the writer
         # ------------------------------------------------------------------------------------
         # writerPass: false if the writer fails to complete creation of output file
         #   - set by the writer
         # ------------------------------------------------------------------------------------
         # writerMessages: an array of writer warning and error messages
         #   - set by the writer
         # ------------------------------------------------------------------------------------
         # writerOutputFormat: format of writer output
         #   - set by the writer
         # ------------------------------------------------------------------------------------
         # writerOutput: the output file returned by the writer
         #   - set by the writer
         # ------------------------------------------------------------------------------------
         # writerForceValid: when required elements are missing from input add placeholder
         #   - set from the parameter list (forceValid)
         # ------------------------------------------------------------------------------------
         # writerShowTags: include tags in XML output for any empty elements
         #   - set from the parameter list (showAllTags)
         # ------------------------------------------------------------------------------------
         # writerCSSlink: CSS link to append to HTML writer output
         #   - set from the parameter list (cssLink)
         # ------------------------------------------------------------------------------------
         # writerMissingIdCount: counter for creating unique element IDs as needed
         #   - set by the writer
         # ------------------------------------------------------------------------------------
         # translatorVersion: current version of the mdTranslator
         #   - set by the translator
         # ------------------------------------------------------------------------------------
