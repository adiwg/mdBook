# mdTranslator

## Architecture

### Internal Object
---
#### coverageInfo:

The *coverageInfo* object contains information about .

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

__dimensionType:__ *string* - type of dimension for the spatial-temporal axis being defined.  Examples: row, column, vertical, line, time, track, ...

