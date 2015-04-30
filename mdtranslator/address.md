# mdTranslator

## Architecture

### Internal Object
---
#### address:

The *address* object contains the individual or organization address for a contact.

````ruby
    def newAddress
        intObj = {
            deliveryPoints: [],
            city: nil,
            adminArea: nil,
            postalCode: nil,
            country: nil,
            eMailList: []
        }
    end
````

__deliveryPoints:__ *array* - an array of quoted strings with each string being a line of the address.  While usually only one or two address lines are needed the number of address lines is not restricted.

__city:__ *string* - name of the city

__adminArea:__ *string* - name of the state or province.  Postal abbreviations for a state or province are also permissable.

__postalCode:__ *string* - postal district code (e.g., zip code in the U.S.).

__country:__ *string* - name of the country or internationally accepted country code.

__eMailList:__ *array* - an array of quoted strings with each string being an email address.
