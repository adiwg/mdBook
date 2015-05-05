# mdTranslator

## Architecture

### Internal Object
---
#### additionalDocumentation:

The *additionalDocumentation* object holds information about other references related to, but not defining, the resource such as  factsheets, data catalog pages, award documents, proposals, and informational websites.

````ruby
    def newAdditionalDocumentation
        intObj = {
            resourceType: nil,
            citation: {}
        }
    end
````

__resourceType:__ *string* - identifies the type of  documentation described by this object. E.g. 'project', 'dataset', 'study', 'publication'.

__citation:__ *object* - a [citation](../mdtranslator/citation.md) object identifying the document including its location.
