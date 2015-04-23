# SRS:

The *SRS* (Spatial Reference System) object defines a specific reference system within a specific [geoElement](../mdtranslator/geoElement.md).  Note that when describing the overall spatial and temporal extent of the larger resource itself, the [spatialReferenceSystem](../mdtranslator/spatialReferenceSystem.md) object should be used instead.

````ruby
    def newSRS
        intObj = {
            srsName: nil,
            srsHref: nil,
            sysType: nil
        }
    end
````

__srsName:__ *string* - the name of the coordinate reference system

__srsHref:__ *URI* - a dereferenceable URI that links to the parameters for the coordinate reference system

__srsType:__ *string* - a string that hints at the format used to represent CRS parameters at the provided URI. Suggested values are: "proj4", "ogcwkt", "esriwkt", but others can be used.
