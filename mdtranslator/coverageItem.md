# mdTranslator

## Architecture

### Internal Object
---
#### coverageItem:

The *coverageItem* object contains information about the .

````ruby
    def newCoverageItem
        intObj = {
            itemName: nil,
            itemType: nil,
            itemDescription: nil,
            minValue: nil,
            maxValue: nil,
            units: nil,
            scaleFactor: nil,
            offset: nil,
            meanValue: nil,
            standardDeviation: nil,
            bitsPerValue: nil,
            classedData: {},
            sensorInfo: {}
        }
    end
````

__itemName:__ *string* - 

__itemType:__ *string* - 