# mdTranslator

## Architecture

### Internal Object
---
#### metadataInfo:

The *metadataInfo:* object contains information about the metadata record itself. This is not the metadata for the resource, that metadata can be found in the [resourceInfo](../mdtranslator/resourceInfo.md) section.
````ruby
    def newMetadataInfo
        intObj = {
            metadataId: {},
            parentMetadata: {},
            metadataCustodians: [],
            metadataCreateDate: {},
            metadataUpdateDate: {},
            metadataURI: nil,
            metadataStatus: nil,
            maintInfo: {},
            extensions: []
        }
    end
````

__metadataId:__ *object* - an object containing the [user provided unique identifier](../mdtranslator/resourceId.md) for the metadata record. The identifier is potentially used by metadata clearinghouses for identification and maintenance of the metadata record. The object is of type resourceId. The citation section of resourceId is ignored in this context.

__parentMetadata:__ *object* - a [citation](../mdtranslator/citation.md) object that identifies the parent metadata for which this metadata record is a subset (child). This might identify a parent project or funding initiative or larger cited data collection.

__metadataCustodians:__ *array* - an array of [responsible party](../mdtranslator/responsibleParty.md) objects for persons or organizations responsible for metadata information.

__metadataCreateDate:__ *object* - a [dateTime](../mdtranslator/dateTime.md) object for the date this metadata record was created.

__metadataUpdateDate:__ *object* - a [dateTime](../mdtranslator/dateTime.md) object for the date the metadata content was last updated.

__metadataURI:__ *string* - Uniform Resource Identifier (URI) of this metadata record.

__metadataStatus:__ *string* - The status of the metadata record; e.g. complete, amended, provisional.

__mainInfo:__ *object* - a [resource maintenance](../mdtranslator/resourceMaint.md) object that provides information about the frequency of metadata updates, and the scope of those updates.

__extensions__ *array* - Information about metadata extensions.  This object is automatically populated for ISO writers requiring the biological extension.
