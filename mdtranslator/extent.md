# mdTranslator

## Architecture

### Internal Object
---
#### extent:

The *extent* object

````ruby
    def newExtent
        intObj = {
            extDesc: nil,
            extGeoElements: [],
            extTempElements: [],
            extVertElements: [],
            extIdElements: []
        }
    end
````

__extDesc:__ *string* - a brief description of the extent

__extGeoElements:__ *array* - an array of [geoElement](../mdtranslator/geoElement.md) objects each describing a geographic boundary or location comprising all or portion of the resource

__extTempElements:__ *array* - an array of [tempElement](../mdtranslator/tempElement.md) objects each describing a temporal boundary comprising all or portion of the resource

__extVertElements:__ *array* - an array of [vertElement](../mdtranslator/vertElement.md) objects each describing a vertical boundary comprising all or portion of the resource

__extIdElements:__ *array* - an array of [geoElement](../mdtranslator/geoElement.md) objects added by the ISO 19115_2 writer to handle identifiers, temporal, or vertical properties describing a geographic object. In ISO these are properties of an extent and not a geography.  Therefore, a new extent is created for each geography with one of these properties defined.  The *extIdElements:* array is not loaded by the reader.
