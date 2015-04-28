# citation:

The *citation:* object contains information that identifies the project, data, publication or other resource being described by the metadata. The *citation* object is used many places throughout the metadata record, so the resource being identified is always dependent on the context in which the citation was placed.

````ruby
    def newCitation
        intObj = {
            citTitle: nil,
            citDate: [],
            citEdition: nil,
            citResourceIds: [],
            citResponsibleParty: [],
            citResourceForms: [],
            citOlResources: []
        }
    end
````

__citTitle:__ *string* (required) - a name for the resource described.

[__citDate:__](../mdtranslator/datetime.html) *object* - the date when the citation was valid for the resource.

__citEdition:__ *string* - edition or version of the resource.

[__citResourceIds:__](../mdtranslator/resourceId.md) *array* - an array of identifiers for the resource.

[__citResponsibleParty:__](../mdtranslator/responsibleParty.md) *array* - an array of people and/or organizations that play a role in the creation, maintenance, or administration of the resource that is of particular interest to the users of this metadata record.

__citResourceForms:__ *array* - an array of strings that describe the forms in which the resource is available (e.g., digitalText, image, or video).

[__citOlResource:__](../mdtranslator/onlineResource.md) *array* - an array of online references related to the resource.
