# Architecture
## Validate

The validation process is one of the reader's responsibilities as it is dependent on the reader's format and standards.

In the example architecture the mdJson validator checks the file structure and syntax by using a JSON parser.  If the file structure is invalid any discernable errors detected by the parser are passed back to the mdTranslator to forward on to the requestor.

If the mdJson file passed to the reader has valid JSON str

