# Translator
##Purpose
ADIwg mdTranslator is a GUI interface for executing the mdTranslator. The mdTranslator converts an input metadata record, written to a known JSON standard, such as the ADIwg JSON standard. It then translates  the metadata into an XML format file, according to a specified standard, such as the ISO 19115-2 standard.

##Interface
The simple interface allows for different means of providing input for translation.

###JSON Input
Three methods of providing input for translation are provided.
+ Upload a file from your local file system
+ Paste the input into the Translator text box
+ Directly write input into the Translator text box

You can submit a completed input, or a snippet of code, such as a contacts section. Note that the snippet must be properly formed with all brackets properly paired, according to the specs anticipated by the Reader.

###Reader
A reader reads the formatted input and validates the input is properly formed relative to the Reader schema. If valid, the input is converted to a universal internal format and passed to the Translator.

Use the drop down box "Choose a Reader..." to specifiy which Reader you wish to use.

###Writer
A writer takes the input that has been "read" into the the Translator and outputs the content as XML, relative to the schema of the specified Writer.

Use the drop down box "Choose a Writer..." to specifiy which Writer you wish to use.

###Validation
Three modes of validation are available.

####Normal
Optional fields left blank are ignored and not output.

####Strict
All fields must be populated with valid content. This mode is primarily used for testing purposes.

####None
This mode turns off validation, allowing the Translator to accept whatever input is provided. Note that this mode may cause the translation to fail or the output to be non-compliant with the specified standard.

###Options
The Output Empty Tags option will direct the Translator to include blank fields in the output. The default behaviour is to filter blank fields in the output for compactness.

The Translate button will provide directions on what information is needed to procede. Once the button displays "Translate!", then click on the button to procede with Translation.

If errors occured in the translation, then messages will appear below the Translate button.
