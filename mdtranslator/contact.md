# mdTranslator

## Architecture

### Internal Object
---
#### contact:

The *contact:* object holds the information about a discrete contact that may be used multiple times throughout the metadata record.

A contact object may describe an individual, an organization, or both.

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

__indName:__ *string* - name of the contact.  A format for the name is enforced.

__orgName:__ *string* - name of the organization.

__position:__ *string* - the position or title of the individual within the organization.

[__phones:__](../mdtranslator/phone.md) *array* - an array of phone numbers associated with the individual and/or organization.

[__address:__](../mdtranslator/address.md) *object* - a mailing or physical address for the individual or organization.

[__onlineRes:__](../mdtranslator/onlineResource.md) *array* - and array of online resources associated with the individual or organization.

__contactInstructions:__ *text* - an open text field to provide any specific information about contacting the individual or organization.
