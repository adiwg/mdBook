# mdTranslator

## Architecture

### Internal Object
---
#### classedData:

The *classedData* object contains information about the thematic classification used with the associated coverage item.

````ruby
    def newClassedData
        intObj = {
            numberOfClasses: nil,
            classedDataItems: []
        }
    end
````

__numberOfClasses:__ *integer* - the number of values used in a thematic classification resource.

__classedDataItems:__ *array* - an array of [classedDataItem](../mdtranslator/classedDataItem.md) objects providing information about a thematic classification item.

