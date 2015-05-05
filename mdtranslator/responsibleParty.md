# mdTranslator

## Architecture

### Internal Object
---
#### responsibleParty:

The *responsibleParty* object contains information about the identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. The *responsibleParty* object is used in many places throughout the metadata record, so the resource being identified is always dependent on the context in which the responsible party was placed.

The *responsibleParty* in the internal object is just a contactId and a role for the contact.  This allows for the re-use of contact information throughout the metadata without re-specification of the contact's information.

````ruby
    def newRespParty
        intObj = {
            contactId: nil,
            roleName: nil
        }
    end
````

__contactId:__ *string* - the unique ID assigned by the metadata author to the given contact in the [contact](../mdtranslator/contact.md) object.

__role:__ *string* - the function of the contact in the current context.
