# mdTranslator

## Architecture

### Internal Object
---
#### spatialReferenceSystem:

The *spatialReferenceSystem* object describes the geospatial referencing system associated with the spatial extent of the data resource. The referencing can be provided indirectly by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. Note that this object is used to describe the overall spatial and extent of the entire resource.  When defining a specific reference system within a [geoElement](../mdtranslator/geoElement.md), the [SRS](../mdtranslator/SRS.md) object should be used instead.

````ruby
    def newSpatialReferenceSystem
        intObj = {
            sRNames: [],
            sREPSGs: [],
            sRWKTs: []
        }
    end
````

__sRNames:__ *array* - an array of quoted strings providing recognized reference system name(s)

__sREPSGs:__ *array* - an array integers providing EPSG Geodetic Parameter Dataset numbers for the reference system, see [epsg-registry.org](http://epsg-registry.org/) for EPSG numbers.

__sRWKTs:__ *array* - an array of quoted Well-known Text (WKT) representation of the reference system(s).
