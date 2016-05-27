# mdTranslator

## Architecture

### Internal Object
---
#### distributor:

The *distributor* object provides information about a distributor and options for obtaining the information resource.

````ruby
    def newDistributor
        intObj = {
            distContact: {},
            distOrderProcs: [],
            distFormats: [],
            distTransOptions: []
        }
    end
````

__distContact:__ *object* - a [responsibleParty](../mdtranslator/responsibleParty.md) object identifying a distributor for the resource

__distOrderProcs:__ *array* - an array of [distOrder](../mdtranslator/distOrder.md) providing information about how the resource may be obtained and related instructions

__distFormats:__ *array* - an array of [resourceFormat](../mdtranslator/resourceFormat.md) objects describing the resource formats available through the distributor

__distTransOptions:__ *array* - an array of [digitalTransOption](../mdtranslator/digitalTransOption.md) objects identifying the technical means and media by which a resource can be obtained from the distributor
