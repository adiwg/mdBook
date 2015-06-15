# mdTranslator

## Architecture

### Internal Object
---
#### resourceInfo:

The *resourceInfo* object contains the metadata that describes the principal resource for this metadata record.  This resource can be a project, dataset, presentation, or any other resource that needs to be described by metadata.

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
            resourceCharacterSets: [],
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

__resourceType:__ *string* - identifies the type of resource described by this metadata. E.g. 'project', 'dataset', 'study', 'publication'.

__citation:__ *object* - a [citation](../mdtranslator/citation.md) object which is the main citation identifying the resource for this metadata record.

__timePeriod:__ *object* - a [time period](../mdtranslator/timePeriod.md) object defining the time span of the resource.  For a project this might the start and end dates.  For a dataset it may be the time span of the data.

__abstract:__ *string* (required) - a brief narrative describing the content of the resource.

__shortAbstract:__ *string* - a short (one or two sentence) version of the abstract which may be used on website popups or lists to introduce the resource.

__hasMapLocation?:__ *true/false* - indicates if the project or resource is tied to a geographic location or area (true).

__hasDataAvailable?:__ *true/false* - indicates if a project has produced data which is available for distribution.

__purpose:__ *string* - a summary of intentions for which the resource was created.

__credits:__ *array* - an array of quoted names of individuals or organizations that made significant contributions to this resource but are not listed in other *responsibleParty* references.

__status:__ *string* - the status of the resource at the time this metadata record was published (e.g., 'complete', 'onGoing', 'suspended').

__pointsOfContact:__ *array* - an array of [responsibleParty](../mdtranslator/responsibleParty.md) objects to identify person(s) and organization(s) that may be contacted for acquiring knowledge about or acquisition of the resource.

__resourceMaint:__ *array* - an array of  [resourceMaint](../mdtranslator/resourceMaint.md) objects that provide information about the maintenance of the resource.

__graphicOverview:__ *array* - an array of [browseGraphic](../mdtranslator/browseGraphic.md) objects the link to images, maps, flow charts, data models, etc. that visually help to describe the resource.

__resourceFormats:__ *array* - an array of [resourceFormat](../mdtranslator/resourceFormat.md) objects that describe the format(s) in which the resource is available.

__resourceLanguages:__ *array* - an array of quoted strings to identify the language(s) and counrty(ies) of origin used within the resource (e.g., 'eng; USA', 'eng; UK', 'esp; MEX').

__resourceCharacterSets:__ *array* - an array of quoted strings to identify the character sets used by the resource (e.g. utf8, utf16, ebcdic).

__descriptiveKeywords:__ *array* - an array of [keyword](../mdtranslator/keyword.md) objects to list relevant keywords and cite the source thesaurus for the keywords.

__resourceUses:__ *array* - an array of [resourceSpecificUsage](../mdtranslator/resourceSpecificUsage.md) objects describing ways in which the resource is currently or has been used, it's limitations, and contact information about a specific usage.

__useConstraints:__ *array* - an array of quoted string statements identifying limitations affecting the fitness for use of the resource. For example, "not to be used for navigation".

__legalConstraints:__ *array* - an array of [legalCon](../mdtranslator/legalCon.md) objects defining the legal constraints regarding the use and access of this resource.

__securityConstraints:__ *array* an array of [securityCon](../mdtranslator/securityCon.md) objects defining the security implications for the use and access of this resource.

__taxonomy:__ *object* - an instance of the [taxonSystem](../mdtranslator/taxonSystem.md) object defining one or more species and the system of taxonomy classification system.

__spatialReferenceSystem:__ *object* - an instance of the [spatialReferenceSystem](../mdtranslator/spatialReferenceSystem.md) object that defines the system used for geospatial data in this resource.

__spatialRepresentationTypes:__ *array* - an array of quoted strings stating the digital mechanism used to
represent spatial information, such as 'vector', 'grid', 'text table,' etc.

__spatialResolutions:__ *array* - an array of [resolution](../mdtranslator/resolution.md) objects providing the geographic scale(s) of the spatial information.

__topicCategories:__ *array* - an array of quotes strings specifying the general theme keyword of the resource, such as 'oceans', 'biota', 'atmosphere'.  Note: for ISO metadata this is a controlled vocabulary codeList.

__environmentDescription:__ *string* - a description of the producer's processing environment, including items such as the software, the computer, and the computer operating system in which the data resource was created.

__extent:__ *array* - an array of [extent](../mdtranslator/extent.md) objects describing the spatial, temporal, and vertical boundaries of the project or data resource.

__dataQualityInfo:__ *array* - an array of [dataQuality](../mdtranslator/dataQuality.md) objects describing the data quality, lineage, and/or processing steps applied to the whole or part of the data resource.

__supplementalInfo:__ *string* - any additional descriptive information about the project or data resource that is covered elsewhere.


