# mdTranslator

## Architecture

### Internal Object
---
#### dimensionInfo:

The *dimensionInfo* object contains information about the spatial-temporal properties of the axis.

````ruby
    def newDimensionInfo
        intObj = {
            dimensionType: nil,
            dimensionTitle: nil,
            dimensionDescription: nil,
            dimensionSize: nil,
            resolution: nil,
            resolutionUnits: nil
        }
    end
````

__dimensionType:__ *string* - type of dimension for the spatial-temporal axis being defined.  Examples: row, column, vertical, line, time, track, ...

__dimensionTitle:__ *string* - name of the axis.

__dimensionDescription:__ *string* - a natural language description of the axis. 

__dimensionSize:__ *integer* - number of elements along the axis.

__resolution:__ *real* - degree of detail in the grid dataset.

__resolutionUnits:__ *string* - units of measure for the grid resolution.
