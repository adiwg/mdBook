# responsibleParty:

The *responsibleParty* object contains information about the identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. The *responsibleParty* object is used many places throughout the metadata record, so the resource being identified is always dependent on context in which the responsible party was placed.

The *resonsibleParty* in the internal object is just a contactId and a role for the contact.  This allows for the reuse of contact information throughout the metadata without respecification of the contact's information.

````ruby
    def newRespParty
        intObj = {
            contactId: nil,
            roleName: nil
        }
    end
````

__contactId:__ *string* - the unique ID the user assigned to the corresponding contact in the [contacts](../mdtranslator/contacts.md) object.

__role:__ *string* - the function of the contact in the current context.
