# contacts:

The *contacts:* array holds the information about individual contacts that will be used throughout the metadata.  Placing contacts in an array allows reuse of a contact multiple times in the metadata without respecifying the contacts information each time it is used.

Contacts can be for an individual an organization, or both.

__contact:__
````ruby
    def newContact
        intObj = {
            contactId: nil,
            indName: nil,
            orgName: nil,
            position: nil,
            phones: [],
            address: {},
            onlineRes: [],
            contactInstructions: nil
        }
    end
````

__contactId:__ *alphaNumeric* (required) - a user provided unique ID for this contact.  This will be used to locate this contact in the contact array.

__indName:__ *alphaNumeric* - name of the contact.  A format for the name is enforced.

__orgName:__ *alphaNumeric* - name of the organization.

__position:__ *alphaNumeric* - the position or title of the individual within the organization.

[__phones:__](../mdtranslator/phone.md) *array* - an array of phone numbers associated with the individual and/or organization.

[__address:__](../mdtranssslator/address.md) *object* - a mailing or physical address for the individual or organization.

[__onlineRes:__](..mdtranslator/onlineResource.md) *array* - and array of online resources associated with the individual or organization.

__contactInstructions:__ *text* - an open text field to provide any specific information about contacting the individual or organization.

---
[base](../mdtranslator/internal_object.md) <br>
[parent](../mdtranslator/internal_object.md)


