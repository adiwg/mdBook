# mdTranslator

## Architecture

### Internal Object
---
#### entity:

The *entity* object provides the definition and schema for a discrete data object within the data resource.  The data object may be a table, dataset, or single sheet of a spreadsheet.

````ruby
    def newEntity
        intObj = {
            entityId: nil,
            entityName: nil,
            entityCode: nil,
            entityAlias: [],
            entityDefinition: nil,
            primaryKey: [],
            indexes: [],
            attributes: [],
            foreignKeys: []
        }
    end
````

__entityId:__ *string* (required) - a user provided unique ID for this entity.  The ID will be used to locate this entity in the entity array

__entityName:__ *string* (required) - the name commonly used to identify this entity

__entityCode:__ *string* - the code name used to identify this entity in a database schema or application software. For spreadsheets this would likely be the sheet name. This items may not be applicable to datasets represented as a file.

__entityAlias:__ *array* - an array of quoted strings providing alternate names used to identify this entity

__entityDefinition:__ *string* (required) - a brief definition for the entity

__primaryKey:__ *array* - an array of quoted [entityAttribute](../mdtranslator/entityAttribute.md) attribute code names that together compose the primary key set for the entity

__indexes:__ *array* - an array of [entityIndex](../mdtranslator/entityIndex.md) objects describing alternate indexes for the entity

__attributes:__ *array* - an array of [entityAttribute](../mdtranslator/entityAttribute.md) objects defining the attributes for the entity

__foreignKeys:__ *array* - an array of [entityForeignKey](../mdtranslator/entityForeignKey.md) objects describing attributes whose values are restricted to values found in the domain of an attribute belonging to another table or dataset
