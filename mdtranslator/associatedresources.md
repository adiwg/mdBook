# associatedResources:

The *associatedResources* object holds information about other references related to, but not describing, the resource such as  factsheets, data catalog pages, award documents, proposal, informational websites.

````ruby
    def newAdditionalDocumentation
        intObj = {
            resourceType: nil,
            citation: {}
        }
    end
````

__resourceType:__ *string* - identifies the type of additional documentation described by this object. E.g. 'project', 'dataset', 'study', 'publication'.

[__citation:__](../mdtranslator/citation.md) *object* - the citation describing the additional document and where it is located.

