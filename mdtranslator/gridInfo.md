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

__dimensions:__ *integer* - the number of independent spatial-temporal axes in the data resource.

__dimensionInfo:__ *array* - an array of [dimensionInfo](../mdtranslator/dimensionInfo.md) objects containing information about properties of the spatial-temporal axis.

__dimensionGeometry:__ *string* - identification of the grid data as a point for cell.

__dimensionTransformParams:__ *Boolean* - indication of whether or not parameters for transformation between image coordinates and geographic or map coordinates exist (are available)
