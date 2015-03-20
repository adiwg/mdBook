# boundingBox:

The *boundingBox* object provides a rectangle that geographicly encompasses that extent of the resource. The bounding box is primarily used to locate resources within a geographic region.

````ruby
    def newBoundingBox
        intObj = {
            westLong: nil,
            eastLong: nil,
            southLat: nil,
            northLat: nil
        }
    end
````

__westLong:__ *number* (required) - the western longitude of the bounding box (-180 < westLong < +180)

__eastLong:__ *number* (required) - the eastern longitude of the bounding box (-180 < eastLong < +180)

__southLat:__ *number* (required) - the southern latitude of the bounding box (-90 < southLat < +90)

__northLat:__ *number* (required) - the northern latitude of the bounding box (-90 < northLat < +90)
