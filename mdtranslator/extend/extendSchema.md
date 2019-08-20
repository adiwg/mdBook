# mdTranslator

## Extending the mdJSON schema

The mdJSON schema, being based in JSON, may be extended without impacting mdTranslator as long as standard mdJSON elements are not renamed, removed, or relocated.  New elements and objects can be added, but they will not be observed by mdTranslator, mdEditor, or any of their readers and writers.  This form of extension may be useful in situations where a user needs to save additional elements to describe special data types or is implementing a local version of mdTranslator.  

To incorporate new elements into the mdJSON standard, more work needs to be done.  

1. Start by posting proposed changed to the schema in a GitHub issue for the mdJson-schemas repository (http://github.com/adiwg/mdJson-schemas/issues).  In the issue include:

   * Name and definition of the containing object
   * Rules associated with the containing object
   * Names and definition for all new elements
   * Rules for all new elements
   * A JSON example of the proposed schema change
   * Include an examples of how the elements will be output in each of the writers if necessary. <br><br>

   Example issue (#230 mdJson-schemas)

   >Class Definition: __standaloneQualityReport__
        "Reference to an external standalone quality report"
   >     
   >Rules:
   >- [ ] optional
   >     
   >---
   >Element Definitions:
   > * reportReference: { citation } "Reference to the associated standalone quality report"
   > * abstract: ( character ) "Abstract for the associated standalone quality report"
   > * elementReport: [ report ] "An array of quality reports"
   > 
   >Rules:
   > - [ ] reportReference: required 
   > - [ ] abstract: required 
   >
   >---
   >mdJson:
   > ````json
   > {
   >   "dataQuality": [
   >      {
   >         "standaloneQualityReport": {
   >            "reportReference": { },
   >            "abstract": "stand alone abstract",
   >            "elementReport": [ ]
   >         }
   >      }
   >   ]
   > }
   > ````
   
1. Update and publish mdJson-schemas 

1. Update and publish mdTools

1. Add the new objects and elements to mdTranslator's internal object, "/lib/adiwg/mdtranslator/internal/internal_metadata_obj.rb".  Objects are added as class methods which can instantiate a new object when building an internal object during a mdTranslator read process.  Example of the phone object:
   ```ruby
    def newPhone
       {
          phoneName: nil,
          phoneNumber: nil,
          phoneServiceTypes: []
       }
    end
   ```
1. Add or modify the object in the mdJson test helpers, "/test/helpers/mdJson_hash_objects.rb".  For new object place a method to instantiate the object and fill all elements with values.  Object elements will be "{}" and array elements "[]".  Values should be valid and predictable.  String elements are given the element name and objects are loaded only when they are required.  In this example "scope" and "citation" are loaded from the "scope" and "citation" methods in this same ruby file. Example:
   ```ruby
    # lineage --------------------------------
    def lineage
       {
          statement: 'statement',
          scope: scope,
          citation: [citation],
          processStep: [],
          source: []
       }
    end
   ```
1. Add or modify mdJson build and add methods in "/test/helpers/mdJson_hash_functions.rb".  When custom values need to be set or optional objects need to be filled, create "build" and "add" methods.  "build" methods return an object, "add" methods insert an object into a passed-in object.  Examples:

   __build methods__
   ````ruby
    def build_date(dateTime, type = 'none')
       hDate = date
       hDate[:date] = dateTime
       hDate[:dateType] = type
       return hDate
    end
   ```` 
   __add methods__
   ````ruby
    def add_email(hContact, email)
       hContact[:electronicMailAddress] = [] unless hContact[:electronicMailAddress]
       hContact[:electronicMailAddress] << email
       return hContact
    end
   ````
1. Extend the mdJson reader to handle the new object and/or elements.

1. Write tests for the mdJson reader extensions and verify they did not cause problems for any other sections of mdJson.

1. Extend the mdJson writer to handle the new object and/or elements.

1. Write tests for the mdJson writer extensions.

1. Extend the HTML writer to display the new object and/or elements.  The HTML writer's purpose is to display all that is contained in the internal object.

1. Extend any existing writers that can support the new object and/or elements. This includes modifying their test scripts as well.  

1. Run rake with all readers and writers to be sure the extension did not cause any unintended issues. 

1. Issue a pull request for the mdJson schema extension. 

1. Extend mdEditor to support the new objects and/or elements.  
