# dataUsage:

The *dataUsage* provides basic information about specific applications for which the resource has/have been or is being used.

````ruby
    def newDataUsage
        intObj = {
            specificUsage: nil,
            userLimits: nil,
            userContacts: []
        }
    end
````

__specificUsage__ *string* - a brief description about how the resource is being used.

_userLimits:__ *string* - a brief description of applications determined by the user for which the resource is not suitable.

__userContacts:__ *array* - an array of [responsibleParty](../mdtranslator/responsibleParty.md) objects identifying persons and/or organizations and their roles using this resource.
