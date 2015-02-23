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

[__distributorInfo:__](../mdtranslator/distributorInfo.md) *array* - contains information about distributors or distribution points for the data or service described by this metadata record.

[__associatedResources:__](../mdtransator/associatedResources.md) *array* - Information about a resource related to the data resource, such as: study, dataset, project, etc. An associated resource may be a child reference, or reference a larger work, such as an initiative.

[__additionalDocuments__](../mdtranslator/additionalDocuments.md) *array* - Additional references associated with the resource, such as: web sites, documents for additional reading, etc.

---
[base](../mdtranslator/internal_object.md) <br>
[parent](../mdtranslator/internal_object.md)
