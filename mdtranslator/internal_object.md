# Internal Object

The *internal object* is Ruby hash containing all the metadata from input file and built up by the reader.  The internal object is flexible in that not all elements, arrays and objects need to be populated but changing the basic structure will likely break all readers.  New items can be added without breaking a writer, but changing element names or deleting a element will require changes to all writers.

The internal object is a collection of nested object all of which are defined in the 'internal_metadata_obj.rb' file.  Object definitions always set initial values to nil, arrays to empty [] and objects to empty {}.

When building or reading an internal object start with the base object 'newBase'.

**base object:**

````ruby
    def newBase
        intObj = {
            schema: {
                name: nil,
                version: nil
            },
            contacts: [],
            metadata: {},
            dataDictionary: {}
        }
    end
````

The base object has 4 sections:

**schema:** *object* (required) - contains the name and version of the metadata input file submitted to the reader.




