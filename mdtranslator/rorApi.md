# mdTranslator

## Architecture

### Ruby on Rails API

The *Ruby on Rails API* is a publicly hosted API interface to the mdTranslator. It is accessible at [http://mdtranslator.adiwg.org/](http://mdtranslator.adiwg.org/).  Complete documentation on version 1.0 of the API is available at [http://mdtranslator.adiwg.org/api/v1](http://mdtranslator.adiwg.org/api/v1). 

The *Ruby on Rails API* provides a RESTful interface to the mdTranslator that passes the metadata content file and other user supplied options to the mdTranslator.  After processing the formatted metadata file is passed back to the user's browser.  There are additional options for formatting the response not available directly from mdTranslator.  The response can be requested as plain text, placed in a JSON or XML wrapper, or as JSONp in addition to the default response format of the writer.  



