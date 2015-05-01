# mdTranslator

## Architecture

### Internal Object
---
#### verticalElement:

The *verticalElement* object describes a vertical range within the extent.

````ruby
    def newVerticalElement
        intObj = {
            minValue: nil,
            maxValue: nil,
            crsURI: nil,
            crsTitle: nil
        }
    end
````

__minValue:__ *number* (required) - the lowest vertical value of the extent

__maxValue:__ *number* (required) - the highest vertical value of the extent

__crsURI:__ *URI* - a web link to the parameters for a geographic reference system associated with a vertical extent

__crsTitle:__ *string* (required) - the name of the geographic reference system associated with a vertical extent
