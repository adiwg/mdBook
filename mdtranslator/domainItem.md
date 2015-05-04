# mdTranslator

## Architecture

### Internal Object
---
#### domainItem:

The *domainItem* object enumerates and defines the valid values for a domain.

````ruby
    def newDomainItem
        intObj = {
            itemName: nil,
            itemValue: nil,
            itemDefinition: nil
        }
    end
````

__itemName:__ *string* - a common name for the domain item

__itemValue:__ *string* (required) - the code or value placed in the dataset attribute to enumerate the domain item

__itemDefinitions:__ *string* - a brief definition for the domain item
