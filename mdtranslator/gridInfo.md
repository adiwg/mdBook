# mdTranslator

## Architecture

### Internal Object
---
#### gridInfo:

The *gridInfo* object contains information about the structure of a gridded data resource.

````ruby
    def newGridInfo
        intObj = {
            dimensions: nil,
            dimensionInfo: [],
            dimensionGeometry: nil,
            dimensionTransformParams: false
        }
    end

````

__dimensions:__ *integer* - 
