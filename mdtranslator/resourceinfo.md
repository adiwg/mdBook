# resourceInfo:

The *resourceInfo* object contains the metadata that describes the principal resource for this metadata record.  This recource can be a project, dataset, presentation, or any other resource that needs to be described by metadata.

````ruby
        intObj = {
            resourceType: nil,
            citation: {},
            timePeriod: {},
            abstract: nil,
            shortAbstract: nil,
            hasMapLocation?: nil,
            hasDataAvailable?: nil,
            purpose: nil,
            credits: [],
            status: nil,
            pointsOfContact: [],
            resourceMaint: [],
            graphicOverview: [],
            resourceFormats: [],
            resourceLanguages: [],
            descriptiveKeywords: [],
            resourceUses: [],
            useConstraints: [],
            legalConstraints: [],
            securityConstraints: [],
            taxonomy: {},
            spatialReferenceSystem: {},
            spatialRepresentationTypes: [],
            spatialResolutions: [],
            topicCategories: [],
            environmentDescription: nil,
            extents: [],
            dataQualityInfo: [],
            supplementalInfo: nil
        }
    end
````

__resourceType:__ *string* -

