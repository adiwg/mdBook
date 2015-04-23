# resourceSpecificUsage:

The *resourceSpecificUsage* object provides basic information about specific application(s) for which the resource(s) has been or is being used by different users.

````ruby
    def newDataUsage
        intObj = {
            specificUsage: nil,
            userLimits: nil,
            userContacts: []
        }
    end
````

__specificUsage:__ *string* (required) - a brief description of the resource usage

__userLimits:__ *string* - a brief description of application(s) for which the provider has determined the resource is not suitable

__userContacts:__ *array* - an array of [responsibleParty](../mdtranslator/responsibleParty.md) objects
