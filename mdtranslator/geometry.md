# geometry:

The *geometry* object

````ruby
    def newGeometry
        intObj = {
            geoType: nil,
            geometry: {},
            dimension: nil
        }
    end
````

__geoType:__ *enumeration* - a text value indicating they type of geometry defined by this object.  Permissible values are: 'BoundingBox', 'Point', 'MultiPoint', 'LineString', 'MultiLineString', 'Polygon', 'MultiPolygon'.  The permissible values are native to GeoJson.

__geometry:__ *object* - an object containing coordinates that define the geometry.  GeoJson notation is used to annotate the coordinates.<br>
examples...<br>
 * Point = '[-160.77777, 45.88888, 500]'
 * MultiPoint = '[[-151.717181, 70.879761], [-134.964531, 41.946544]]'
 * LineString = '[[-120.71, 70.87], [-130.96, 41.94], [-140.32, 87.12]]'
 * MultiLineString = '[[[-120, 70], [-130, 41], [-140, 87]], [[-125, 70], [-135, 60], [-145, 50]]]'
 * Polygon = a [polygonSet](../mdtranslator/polygonSet.md) object containing the coordinates for the polygon and any exclusion rings
 * MultiPolygon = an array of [polygonSet](../mdtranslator/polygonSet.md) objects containing the coordinates for the polygons and any exclusion rings

__dimension:__ *integer* - indicates the number of dimensions in a coordinate. i.e. (x,y) = 2; (x,y,z) = 3; (x,y,z,t) = 4
