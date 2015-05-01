# mdTranslator

## Architecture

### Internal Object
---
#### entityIndex:

The *entityIndex* object that defines an alternate index for the entity - an index other than the primary key.  In SQL this would be implemented using a CREATE INDEX statement.

````ruby
    def newEntityIndex
        intObj = {
            indexCode: nil,
            duplicate: false,
            attributeNames: []
        }
    end
````

__indexCode:__ *string* (required) - the code name used to define the alternate index on the entity

__duplicate:__ *boolean* (required) - indicates whether the index allows duplicates or values are required to be unique.  true = allow duplicates; false = values must be unique.

__attributeNames:__ *array* (required) - an array of quoted attribute code names that together compose an alternate key set for the entity
