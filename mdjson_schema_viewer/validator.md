# Validator
##Purpose
ADIwg mdJSON Validator is a tool to test a metadata file written in the ADIwg JSON standard for valid input. The validator tests for valid JSON format and conformance to the ADIwg JSON schema. The Validator is handy for testing your metadata file before running the Translator.
##Interface
The simple interface allows for different means of providing ADIwg JSON for testing.
###JSON Input
Three methods of providing ADIwg JSON are provided.
+ Upload a file from your local file system
+ Paste ADIwg JSON into the Validator text box
+ Directly write ADIwg JSON into the Validator text box

Once an input is provided, clicking on the "Validate!" button will execute the Validator.

You can submit a completed ADIwg JSON metadata record, or a snippet of code, such as just the contacts section. Note that the snippet must be properly formed with all brackets properly paired.

###Options
The Validator can be run with the following options:

####Strict
Clicking on Strict runs the JSON input validating that all fields are populated. Non-Strict mode allows empty elements in the input.

####Stop at First Error
Tells the Validator to cease processing at the first error encountered. In this manner one may step through errors, making corrections along the way. Without the Stop option, the Validator will process the entire input.

###Errors
If any errors are encountered by the Validator, a display of the errors are listed. If the JSON could not be parsed, then a popup window will indicate invalid syntax. Click outside the popup to continue.

If the errors were due to a problem with the structure of the metadata, then an error report window appears below the "Validate!" button.

Clicking the "+" icon will expand the error message for more detailed information.

Note that an error location in the input is not highlighted in the Validator text box, nor is the location revealed in the error report.

If locating the source of the error becomes too difficult, it may help to run a sub-set of the input to attempt to isolate the source of the error.

Common errors involve involve improper pairing of brackets. For instance, a missing bracket or invalid bracket type. See the mdJSON topic for more information.
