# Validator

##Purpose
ADIwg mdJSON Validator is a tool to test a metadata file written in the ADIwg JSON standard for valid input. The validator tests for valid JSON format and conformance to the ADIwg JSON schema. The Validator is handy for testing your metadata file before running the Translator.

##Interface
The simple interface allows for different means of providing ADIwg JSON for testing.

###JSON Input
Three methods to input ADIwg JSON are provided.
+ Upload a file from your local file system
+ Paste ADIwg JSON into the Validator text box
+ Directly write ADIwg JSON into the Validator text box

Once an input is provided, clicking on the "Validate!" button will execute the Validator.

The input metadata record does not need to be fully completed, but needs to be in a valid structure and contain the minimum elements. To see an example of minimal valid input, click on the "Load Example" link immediately below the Validator text box.

###Options
The Validator can be run with the following options:

####Strict
Clicking on Strict runs the JSON input validating that all content is valid. Non-Strict mode is more permissive, ignoring unrecongizable content.

####Stop at First Error
Tells the Validator to cease processing at the first error encountered. In this manner, one may step through errors, making corrections along the way. Without the Stop option, the Validator will process the entire input.

###Errors
If the input passed validation, a confirmation message is displayed.

If any errors are encountered by the Validator, a display of the errors are listed. If the JSON could not be parsed, indicating improperly formed JSON, then a popup window will indicate invalid syntax, along with the syntax in question. Click outside the popup to continue.

If the input JSON is properly formed, but errors were encountered relative to the ADIwg schema, then an error report window appears below the "Validate!" button. This report will list errors relative to the options chosen. If "Stop at First Error" is on, then the first encountered error is displayed. Otherwise, all errors encountered are listed.

Clicking the "+" icon will expand the error message for more detailed information.

Expanding the error icon shows three sections, Message, Data Path and Schema Path.

+ Message is the error message.
+ Data Path is the element location in the input where the error was encountered.
+ Schema Path shows the schema pathname to the location where the error was encountered. Using the Viewer, you can navigate to that location for more information.

Note that an error location in the input is not highlighted in the Validator text box.

The error may contain "sub-errors". These errors are secondary errors that were encountered in relation to the primary error. These errors may provide more clues as to the source of the problem.

Common errors may include improper pairing of brackets. For instance, a missing bracket or invalid bracket type (See the mdJSON topic for more information).
