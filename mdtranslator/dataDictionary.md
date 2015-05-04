# mdTranslator

## Architecture

### Internal Object
---
#### dataDictionary:

The *dataDictionary* object contains a description objects describing the collection of physical objects or items in a data resource (schema). This is a description of the physical structure of the data rather than its meaning.

````ruby
    def newDataDictionary
        intObj = {
            dictionaryInfo: {},
            domains: [],
            entities: []
        }
    end
````

[__dictionaryInfo:__](../mdtranslator/dictionaryInfo.md) *object* - an object that contains identification, descriptive, and contact information for the data dictionary.

__domains:__ *array* - an array of [dictionaryDomain](../mdtranslator/dictionaryDomain.md) objects that define a list of permissable values used to constrain an attribute's value.  A single domain may be assigned to multiple attributes in a table or database.

__entities:__ *array* - an array of [entity](../mdtranslator/entity.md) objects that defines the structure of a discrete data object within the data resource.  The data object may be a table, dataset, or single sheet of a spreadsheet.