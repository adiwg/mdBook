# mdTranslator

## Architecture

### Internal Object
---
#### timeInstant:

The *timeInstant* object is a dateTime associated with an ID and description.

````ruby
    def newTimeInstant
        intObj = {
            timeId: nil,
            description: nil,
            timePosition: {}
        }
    end
````

__timeId:__ *string* - a user provided unique identifier for the *timeInstant*

__description:__ *string* - a brief description providing relevant information about the date and time

__timePosition:__ *object* (required) - a [dateTime](../mdtranslator/dateTime.md) object providing the date and time for the *timeInstant*
