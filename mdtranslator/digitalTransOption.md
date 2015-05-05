# mdTranslator

## Architecture

### Internal Object
---
#### digitalTransOption:

The *digitalTransOption* object identifies a technical means and media by which a resource can be obtained from the associated distributor.  Note that there is some confusion in naming caused by the ISO 19115 naming of this object.  The ISO name for this class is 'MD_digitalTransferOptions' and the ISO wrapper is 'distributorTransferOptions'.  *distributor* was used in the mdJson schema and *digital* was used in the mdTranslator internal object.

````ruby
    def newDigitalTransOption
        intObj = {
            online: [],
            offline: {}
        }
    end
````

__online:__ *array* - an array of [onlineResource](../mdtranslator/onlineResource.md) objects that provide information about online sources from which the resource can be obtained.

__offline:__ *object* - a [medium](../mdtranslator/medium.md) object that provides information about offline media on which the resource can be obtained.
