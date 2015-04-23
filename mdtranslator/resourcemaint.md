# resourceMaint:

The *resourceMaint* object contains information about the maintenance of the resource being described.  The *resourceMaint* object is used many places throughout the metadata record, so the maintenance being described is always dependent on context in which the maintenance object was placed.

````ruby
    def newResourceMaint
        intObj = {
            maintFreq: nil,
            maintNotes: [],
            maintContacts: []
        }
    end
````

__maintFreq:__ *string* - a description of the scheduled update frequency for the resource (e.g., 'monthly, 'annually', 'not scheduled').

__maintNotes:__ *array* - an array of quoted string statements providing information about the maintenance of this resource.

__maintContacts:__ *array* - an array of [responsibleParty](../mdtranslator/responsibleParty.md) objects identifying people and/or organizations in their roles for maintaining the resource being described.
