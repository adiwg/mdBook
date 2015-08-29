# mdTranslator

## Architecture

### Internal Object
---
#### classedDataItem:

The *classedDataItem* object contains information about the thematic classification item.

````ruby
    def newClassedDataItem
        intObj = {
            className: nil,
            classDescription: nil,
            classValue: nil
        }
    end
````

__className:__ *string* - name of the thematic classification item.

__classDescription:__ *string* - a natural language description of the thematic classification item. 

__classValue:__ *string* - the thematic classification value.
