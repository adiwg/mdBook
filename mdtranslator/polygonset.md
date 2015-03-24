# polygonSet:

The *polygonSet* object

````ruby
    def newPolygonSet
        intObj = {
            exteriorRing: {},
            exclusionRings: []
        }
    end
````

__exteriorRing:__ *object* (required) - an object containing coordinates that define the exterior polygon ring. GeoJson notation is used to annotate the coordinates.  The final point in the polygon ring must be the same as the first to close the ring. <br>
example...<br>
 * [[-139.11, 59.82], [-140.11, 59.83], [-143.11, 60.22], [-147.11, 60.82], [-148.11, 59.98], [-148.11, 57.94], [-134.11, 57.66], [-139.11, 59.82]]

__exclusionRings:__ *array* - an array of coordinate sets defining any exclusion polygons within the exterior polygon. GeoJson notation is used to annotate the coordinates.  The final point in each polygon ring must be the same as the first to close the ring. <br>
examples...<br>
 * []
 * [<br>[[-139.3, 59.8], [-140.3, 59.8], [-148.3, 57.9], [-134.3, 57.6], [-139.3, 59.8]], <br>[[-139.4, 59.8], [-147.4, 60.8], [-148.4, 59.9], [-148.4, 57.9], [-134.4, 57.6],[-139.4, 59.8] ]<br>]
