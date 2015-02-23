# metadataInfo:

The *metadataInfo:* object contains information about the metadata record itself.

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

[__metadataId:__](../mdtranslator/resourceid.md) *object* - a user provided unique identifier for the metadata record. The identifier is potentially used by metadata clearinghouses for identification and maintenance of the metadata record. The object is of type resourceId. The citation section of resourceId is ignored in this context.

[__parentMetadata:__](../mdtranslator/citation.md) *object* - Identifies the metadata to which this metadata record is a subset (child). This might identify a parent project or funding initiative or larger cited data collection.

[__metadataCustodians:__](../mdtranslator/responsibleParty.md) *array* - Persons or organizations responsible for metadata information.

[__metadataCreateDate:__](../mdtranslator/dateTime.md) *object* - the date this metadata record was created.

[__metadataUpdateDate:__](../mdtranslator/dateTime.md) *object* - the date the metadata content was last updated.

__metadataURI:__ *string* - Uniform Resource Identifier (URI) of this metadata record.

__metadataStatus:__ *string* - The status of the metadata record; e.g. complete, ammended, provisional.

[__mainInfo:__](../mdtranslator/resourceMaint.md) *object* - Provides information about the frequency of metadata updates, and the scope of those updates.

__extensions__ *array* - Information about metadata extensions.  This objects is automatically populated for ISO writers requiring the biological extension.

---
[base](../mdtranslator/internal_object.md) <br>
[parent](../mdtranslator/metadata.md)

