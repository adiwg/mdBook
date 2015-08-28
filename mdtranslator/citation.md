# mdTranslator

## Architecture

### Internal Object
---
#### citation:

The *citation:* object contains information that identifies the project, data, publication or other resource being described by the metadata. The *citation* object is used many places throughout the metadata record, so the resource being identified is always dependent on the context in which the citation was placed.

````ruby
    def newCitation
        intObj = {
            citTitle: nil,
            citAltTitle: nil,
            citDate: [],
            citEdition: nil,
            citResourceIds: [],
            citResponsibleParty: [],
            citResourceForms: [],
            citOlResources: []
        }
    end
````

__citTitle:__ *string* (required) - a name for the resource being described.

__citAltTitle:__ *string* - an alternate or more descriptive title for the resource being rescribed.

__citDate:__ *object* - a [dateTime](../mdtranslator/datetime.md) object for the date when the citation was valid for the resource.

__citEdition:__ *string* - edition or version of the resource.

__citResourceIds:__ *array* - an array of [resourceId](../mdtranslator/resourceId.md) objects containing identifier for the resource. 

__citResponsibleParty:__ *array* - an array of [responsibleParty](../mdtranslator/responsibleParty.md) objects identifying people and/or organizations that play a role in the creation, maintenance, or administration of the resource that is of particular interest to the users of this metadata record.

__citResourceForms:__ *array* - an array of strings that describe the forms in which the resource is available (e.g., digitalText, image, or video).

__citOlResource:__ *array* - an array of [onlineResource](../mdtranslator/onlineResource.md) objects related to the resource.
