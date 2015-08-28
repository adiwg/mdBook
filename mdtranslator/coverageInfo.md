# mdTranslator

## Architecture

### Internal Object
---
#### coverageInfo:

The *coverageInfo* object contains information about the content of grid cells.

````ruby
    def newCoverageInfo
        intObj = {
            coverageType: nil,
            coverageName: nil,
            coverageDescription: nil,
            processingLevel: {},
            coverageItems: [],
            imageInfo: {}
        }
    end
````

__coverageType:__ *string* - type of information represented by the cell value. Example: image, thematic classification, physical measurement...

__coverageName:__ *string* - name of the coverage.

__coverageDescription:__ *string* - a natural language description of the coverage.

__processingLevel:__ *object* - a [resourceId](../mdtranslator/resourceId.md) object identifying the image distributor’s code that identifies the level of radiometric and geometric processing applied to the coverage.

__coverageItems:__ *array* - an array of [coverageItem](../mdtranslator/coverageItem.md) providing information about the item described by the grid cell.

__imageInfo:__ *object* - a [imageInfo](../mdtranslator/imageInfo.md) object providing information about the image.
