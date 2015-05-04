# mdTranslator

## Architecture

### Internal Object
---
#### timePeriod:

The *timePeriod* object identifies a period of time relevant to the extent.  The nature of the relevancy is provided in the description element of the *timePeriod*.

````ruby
    def newTimePeriod
        intObj = {
            timeId: nil,
            description: nil,
            beginTime: {},
            endTime: {}
        }
    end
````

__timeId:__ *string* - a user provided unique identifier for the *timePeriod*

__description:__ *string* - a brief description providing relevant information about the datetime period

__beginTime:__ *object* - a [dateTime](../mdtranslator/dateTime.md) object providing the date and time for the begining of the time period

__endTime:__ *object* - a [dateTime](../mdtranslator/dateTime.md) object providing the date and time for the end of the time period
