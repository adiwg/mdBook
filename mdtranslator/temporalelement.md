# mdTranslator

## Architecture

### Internal Object
---
#### temporalElement:

The *temporalElement* object provides the temporal context for the extent.  The *temporalElement* can be either a date, time instant, or time period.

````ruby
    def newTemporalElement
        intObj = {
            date: {},
            timeInstant: {},
            timePeriod: {}
        }
    end
````

__date:__ *object* - a [dateTime](../mdtranslator.md) object providing a date and time

__timeInstant:__ *object* - a [timeInstant](../mdtranslator/timeInstant.md) object providing additional ID and descriptive information about the dateTime

__timePeriod:__ *object* - a [timePeriod](../mdtranslator/timePeriod.md) object identifies a period of time relevant to the extent.
