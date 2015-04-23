# resolution:

The *resolution* object factor which provides a general understanding of the density of spatial data in the dataset.  Either the equivalent scale is required or the distance/distanceUOM is required, but not both.  Although both are allowed in the resolution object.

````ruby
    def newResolution
        intObj = {
            equivalentScale: nil,
            distance: nil,
            distanceUOM: nil
        }
    end
````

__equivalentScale:__ *number* - the scale of geographic extent expressed as the denominator of map scale (e.g., 250000 = 1:250,000 map scale).

__distance:__ *number* - the ground distance measurement representing geographic extent

__distanceUOM:__ *string* - the ground distance unit of measure
