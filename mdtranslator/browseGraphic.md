# mdTranslator

## Architecture

### Internal Object
---
#### browseGraphic:

The *browseGraphic* object provides a link to an image, map, flow chart, data model, etc. that visually help to understand the resource.

````ruby
    def newBrowseGraphic
        intObj = {
            bGName: nil,
            bGDescription: nil,
            bGType: nil,
            bGURI: nil
        }
    end
````

__bGName:__ *string* - name of the file that contains a browse graphic.

__bGDescription:__ *string* - a brief description of the browse graphic.

__bGType:__ *string* - the format in which the illustration is encoded such as GIF, JPEG, PBM, PS, TIFF.

__bGURI:__ *string* - a web link to the browseGraphic.
