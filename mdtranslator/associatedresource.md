# associatedResource:

The *associatedResource* object contains informatino on resources which have some direct lineage to the central resource of this metadata such as parent or child datasets or projects.

````ruby
    def newAssociatedResource
        intObj = {
            associationType: nil,
            initiativeType: nil,
            resourceType: nil,
            resourceCitation: {},
            metadataCitation: {}
        }
    end
````

__associationType:__ *string* - identifies how the associated resource is related to the central resource such as 'is a component of', 'larger work citation', 'sub-project', etc.

__initiativeType:__ *string* - identifies type of initiative under which the resource was produced such as 'study', 'task', 'experiment', 'sensor'.

__resourceType:__ *string* - identifies the type of  resource described by this object. E.g. 'project', 'dataset', 'study', 'publication'.

__resourceCitation:__ *object* - a [citation](../mdtranslator/citation.md) object identifying the resource including its location.

__metadataCitation:__ *object* - a [citation](../mdtranslator/citation.md) object identifying the metadata record for the resource including its location.
