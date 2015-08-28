# mdTranslator

## Architecture

### Internal Object
---
#### coverageItem:

The *coverageItem* object contains information about the content of a grid cell.

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

__itemName:__ *string* - the coverage item name

__itemType:__ *string* - the type of value in the grid cell.  Example: real, integer, binary...

__itemDescription:__ *string* - a natural language description of the coverage item.

__minValue:__ *real* - the minimum value of data values in the domain of the coverage item.

__maxValue:__ *real* - the maximum value of data values in the domain of the coverage item.

__units:__ *string* - units for the data in which the coverage item is expressed.

__scaleFactor:__ *real* - scale factor which has been applied to the coverage item.

__offset:__ *real* - the physical value corresponding to a coverage item value of zero.

__meanValue:__ *real* - mean value of data values in the coverage item.

__standardDeviation__ *real* - standard deviation of data values in the coverage item.

__bitsPerValue:__ *integer* - maximum number of significant bits in the uncompressed representation for the value in each pixel.

__classedData:__ *object* - a [classedData](../mdtranslator/classedData.md) object providing information about the thematic classification used with this coverage item. 

__sensorInfo:__ *object* - a [sensorInfo](../mdtranlator/sensorInfo.md) object providing information about the sensor that collected the grid cell values.
