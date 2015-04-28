# Internal Object

The *internal object* is implemented in a Ruby hash and contains all the metadata from the input file and built up by the Reader. The internal object is flexible in that not all elements, arrays and objects must be populated, but changing the basic structure will likely break any Readers or Writers developed against the original hash structure, so this should be done with care. New items can be added without breaking a Writer, but changing element names or deleting an element will require changes to all Writers.

The *internal object* is a collection of nested hash objects assembled in the Reader by instancing and loading hash objects as they are required by the Reader.  All the hash objects are defined in the 'internal_metadata_obj.rb' file.  A newly instanced hash object always sets initial string and numeric values to nil, arrays to empty [], and objects to empty {}.

When building or reading an internal object, start with the base object 'newBase'.

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
            dataDictionary: []
        }
    end
````

The base object has 4 sections:

**schema:** *object* (required) - contains the schema name and version for the metadata input file submitted to the reader.

> __name:__ *string* (required) - name of the encoding schema used by the input metadata file submitted to the reader.
>
> __version:__ *string* (required) - version of the encoding schema used

__contacts:__ *array* - holds an array of [contact](../contact.md) objects.  The internal object stores information about a contact in an array so the contact can be stored once and reused multiple times throughout the metadata record.

[**metadata:**](../mdtranslator/metadata.md) *object* - holds a hash object containing the metadata for the resource being described, generally a project or data resource.

__dataDictionary__ *array* - an array of [dataDictionary](../mdtranslator/dataDictionary.md) objects describing the collection of physical objects or items in a data resource (schema).


