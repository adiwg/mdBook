# Translator
##Purpose
ADIwg mdTranslator is a GUI interface for executing the mdTranslator. The mdTranslator converts an input metadata record, written to a known JSON standard, such as the ADIwg JSON standard. It then translates  the metadata into an XML format, according to a specified standard, such as the ISO 19115-2 standard.

##Interface
The simple interface allows for different means of providing input for translation and a choice of JSON schema readers and XML writers.

###JSON Input
Three methods of input for translation are provided.
+ Upload a file from your local file system
+ Paste the input into the Translator text box
+ Directly write input into the Translator text box

The input metadata record does not need to be fully completed, but needs to be in a valid structure and contain the minimum elements. To see an example of minimal valid input, click on the "Load Example" link immediately below the Translator text box. This is an example of ADIwg JSON intended for the ISO 19115-2 writer. Note, the input must be valid relative to the JSON reader you intend to use.

###Reader
A Reader reads the input and validates that the input is properly formed relative to the Reader schema. If valid, the input is passed to the Translator.

Use the drop down box "Choose a Reader..." to specify which Reader you wish to use. The selected Reader should match the format of the input metadata file.

###Writer
A Writer takes the input that has been "read" into the Translator and outputs the content as XML, relative to the schema of the specified Writer.

Use the drop down box "Choose a Writer..." to specify which Writer you wish to use. The selected Writer will dictate the format of the output metadata file.

###Validation
Three modes of validation are available, Normal, Strict and None.

####Normal
Optional elements left blank are ignored and not output.

####Strict
All fields must be populated with valid content. This mode is primarily used for testing purposes.

####None
This mode turns off validation, allowing the Translator to accept whatever input is provided. Note that this mode may cause the translation to fail or the output to be non-compliant with the specified standard.

###Options
The Output Empty Tags option will direct the Translator to include blank elements in the output. The default behavior is to filter blank elements in the output for compactness.

The Translate button will provide directions on what information is needed as input to the Translator, through informative text displayed on the button. Once the button displays "Translate!", then all required input has been provided, click on the button to proceed with translation.

###Output
If the input was successfully translated, then the output XML will display below the "Translate!" button. The output can be perused for verification.

An "Open in New Window" button is available immediately below the "Translate!" button. Clicking on this button will display the output in a separate browser window.

###Errors
If any errors are encountered by the Translator, a display of the errors are listed. If the JSON could not be parsed, indicating improperly formed JSON, then a popup window will indicate invalid syntax and identify the syntax problem. Click outside the popup to continue.

If the input JSON is properly formed, but errors were encountered relative to the Reader schema, then an error report window appears below the "Translate!" button. This report will list all errors encountered relative to the options chosen.

Clicking the "+" icon will expand an error message for more detailed information.

Expanding the error icon shows three sections, Message, Data Path and Schema Path.

+ Message is the error message.
+ Data Path is the element location in the input where the error was encountered.
+ Schema Path shows the schema pathname to the location where the error was encountered. Using the Viewer, you can navigate to that location for more information.

Note that an error location in the input is not highlighted in the Translator text box.

The error may contain "sub-errors". These are secondary errors that were encountered in relation to the primary error. These errors may provide more clues as to the source of the problem.

Common errors may include improper pairing of brackets. For instance, a missing bracket or invalid bracket type (See the mdJSON topic for more information).

