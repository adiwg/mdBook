# resourceId:

The *resourceId* object contains information about identifiers associated with a resource. Identifiers can be in many forms including acronyms, uuids, alternate names, or database keys.  They can be used to include any names or codes which a project or data resources may be known by.

````ruby
    def newResourceId
        intObj = {
            identifier: nil,
            identifierType: nil,
            identifierCitation: {}
        }
    end
````
__identifier:__ *string* (required) - the identifier.

__identifierType:__ *string* - the type of identifier such as uuid, acronym, or something specific like 'Global Terrestrial Permafrost Network ID'.

[__citation:__](../mdtranslator/citation.md) *object* - an optional citation to cite the source or issuing agency of a particular identifier.
