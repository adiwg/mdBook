# mdTranslator

## Architecture

### Internal Object
---
#### dictionaryDomain:

The *dictionaryDomain* object contains a list of permissable values used to constrain an attribute's value.  A single domain list may be assigned to multiple attributes in a database or even in a single table.

````ruby
    def newDictionaryDomain
        intObj = {
            domainId: nil,
            domainName: nil,
            domainCode: nil,
            domainDescription: nil,
            domainItems: []
        }
    end
````

__domainId:__ *string* (required) - a user provided unique ID for this domain.  The ID will be used to locate the domain in the domain array.

__domainName:__ *string* - a short common name for the domain.

__domainCode:__ *string* - the code or 'lookup table' name for the domin used in the database schema definitions.

__domainDescription:__ *string* - a brief description of the domain including identification of any established sources used in creating the list of domain items.

__domainItems:__ *array* (required) - an array of [domainItem](../mdtranslator/domainItem.md) objects that enumerate and define the valid values for a domain.
