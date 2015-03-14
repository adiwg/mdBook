# metadata:

The *metadata:* object holds the body of the metadata for the resource.  It is organized into the 5 major sections defined below.

````ruby
    def newMetadata
        intObj ={
            metadataInfo: {},
            resourceInfo: {},
            distributorInfo: [],
            associatedResources: [],
            additionalDocuments: []
        }
    end
````

[__metadataInfo:__](../mdtranslator/metadataInfo.md) *object* - contains information about the metadata record itself.

[__resourceInfo:__](../mdtranslator/resourceInfo.md) *object* - contains metadata for the resource being described by this metadata record.

__distributorInfo:__ *array* - an array of  [distributor](../mdtranslator/distributor.md) objects information about distributors or distribution points for the data or service described by this metadata record.

__associatedResources:__ *array* - an array of [associatedResources](../mdtransator/associatedResource.md) objects referencing resources which have some direct lineage to the central resource of this metadata such as parent or child datasets or projects.

__additionalDocuments:__ *array* - an array of  [additionalDocumentation](../mdtranslator/additionalDocumentation.md) objects identifying other documents related to, but not defining, the resource such as  factsheets, data catalog pages, award documents, proposal, informational websites.
