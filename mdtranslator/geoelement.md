# geoElement:

The *geoElement* object

````ruby
    def newGeoElement
        intObj = {
            elementId: nil,
            elementIncludeData: nil,
            elementName: nil,
            elementDescription: nil,
            temporalElements: [],
            verticalElements: [],
            elementIdentifiers: [],
            elementScope: nil,
            elementAcquisition: nil,
            elementSrs: {},
            elementGeometry: {}
        }
    end
````

__elementId:__ *string* - a unique ID assigned by the user to identify this geographic element

__elementIncludeData:__ *boolean* - indicates if the boundary of the geographic element encompasses the resource or excludes the resource.  true = encompasses resource; false = excludes resource

__elementName:__ *string* - a user assigned name for the geographic element

__elementDescription:__ *string* - a brief description of the geographic element

__teporalElements:__ *array* - an array of [temporalElement](../mdtranslator/temporalElement.md) objects each describing a temporal boundary comprising all or portion of the geographic element

__verticalElements:__ *array* - an array of [verticalElement](../mdtranslator/verticalElement.md) objects each describing a vertical boundary comprising all or portion of the geographic element

__elementIdentifiers:__ *array* - an array of [resourceId](../mdtranslator/resourceId.md) objects each defining an identifier assigned to this geographic element

__elementScope:__ *string* - a brief statement describing the portion of the extent covered by this geographic element

__elementAcquisition:__ *string* - a brief statement of the method used to determine the position of the geographic element

__elementSrs:__ *object* - an [SRS](../mdtranslator/SRS.md) object describing the spatial reference system for the geographic element

__elementGeometry:__ *object* (required) - a [geometry](../mdtranslator/geometry.md) object that can describe a boundingBox, point, lineString, or polygon.
