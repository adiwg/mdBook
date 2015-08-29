# mdTranslator

## Architecture

### Internal Object
---
#### locale:

The *locale* object contains information about the sensor that collected the grid cell values.

````ruby
    def newLocale
        intObj = {
            languageCode: nil,
            countryCode: nil,
            characterEncoding: nil
        }
    end
````

__languageCode:__ *string* - the name of the language preferable using the ISO 639-2 code list maintained by the Library of Congress.

__countryCode:__ *string* - the name of the country preferable using the ISO 3166-1 alpha-3 code list. 

__characterEncoding:__ *string* - character encoding system used; generally 'utf8'.  
