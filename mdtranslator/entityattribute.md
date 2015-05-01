# mdTranslator

## Architecture

### Internal Object
---
#### entityAttribute:

The *entityAttribute* object defines a unique member of the entity.  Entity attributes correspond to the columns of database tables and columns of a spreadsheets. Both the entity attribute and its properties are described by this object.

````ruby
    def newEntityAttribute
        intObj = {
            attributeName: nil,
            attributeCode: nil,
            attributeAlias: [],
            attributeDefinition: nil,
            dataType: nil,
            allowNull: true,
            unitOfMeasure: nil,
            domainId: nil,
            minValue: nil,
            maxValue: nil
        }
    end
````

__attributeName:__ *string* (required) - the common name used to identify this attribute

__attributeCode:__ *string* (required) - the code used to identify this attribute.  Most often this will be the table or spreadsheet column name

__attributeAlias:__ *array* - an array of quoted strings providing alternate names by which the attribute is known

__attributeDefinition:__ *string* (required) - a succinct but comprehensive definition for the attribute

__dataType:__ *string* - the datatype for the attribute.  Names for datatypes vary widely by database management system.  Use the datatype name associated with the database system that implemented the entity (e.g., 'integer', 'boolean', 'decimal(8,5)', 'varchar(200)').

__allowNull:__ *boolean* - indicates whether null values are allowed for the attribute

__unitOfMeasure:__ *string* - a unit-of-measure for the attribute (e.g., 'meters', 'atmospheres', 'liters').

__domainId:__ *string* - provides the domain ID for the [dictionaryDomain](../mdtranslator/dictionaryDomain.md) containing the list of permissable values for this attribute

__minValue:__ *string* - the minimum range value permissible for this attribute

__maxValue:__ *string* - the maximum range value permissible for this attribute
