# JSON Schemas

Please note: clicking on any of the individual components below will route a user to an online example JSON file.

### [citation](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/citation.json)

The citation.json schema file defines the structure of the citation block of ADIwg metadata in its native JSON format. This section of the metadata is used to reference published or unpublished data and informational products that pertain to the data or effort described in the metadata record. Uses of the citation schema in ADIwg metadata typically include one or more citations for the dataset or sampling effort described by the metadata; references to authorities responsible for any taxonomies or controlled vocabularies used in the metadata; and to provide a reference to a data or processing-step source in the dataset lineage.

The citation schema is referenced by the dataQuality.json, keyword.json, metadata.json, and taxonomy.json schemas. This schema references the contact.json schema and definitions from schema.json.

### [contact](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/contact.json)

The contact.json schema defines the structure of the contact block of ADIwg metadata in its native JSON format. This section of the metadata is used to provide credit to the individuals and organizations responsible for funding,
collecting, processing, managing, or preserving the data during some part of the data lifecycle. For each individual or organization listed as a contact, this schema defines the metadata elements describing the names, physical and email addresses, position titles, phone numbers and types, online resource information and formats, and the role of each contact in the data lifecycle.

The contact.json schema is directly referenced by the citation.json, dataQuality.json, distibutor.json, metadata.json, maintInfo.json, resourceInfo.json, taxonomy.json, and usage.json JSON schemas.

### [dataQuality](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/dataQuality.json)

The dataQuality.json schema defines the structure of the data quality block of ADIwg metadata in its native JSON format. This section of the metadata describes the lineage of the project or data resource decribed by the metadata record. This history of the resource is modeled in terms of process steps and sources. Process steps provide elements describing a rationale, narrative description, process date, and processor point of contact elements. Sources are described with a narrative description, a reference to a citation block describing the source or a metadata record describing the source, and a reference to a process step performed on the source.

The dataQuality schema is referenced by resourceInfo.json. This schema references the citation.json and contact.json schemas.

### [distibutor](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/distributor.json)

The distributor.json schema defines the structure of the distributor block of ADIwg metadata in its native JSON format. The distributor block provides information on the means of delivery available for the resource, the formats in which the resource is available, and references the points of contact for the distributors of the resource.

This schema references the contact.json and onlineResource.json schemas, and is referenced by the metadata.json and resourceInfo.json schemas.

### [extent](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/extent.json)

The extent.json schema defines the structure of the extent block of ADIwg metadata in its native JSON format. The extent block describes the spatial regions and time periods that are relevant to the areas and periods of data collection and the descriptive breadth of the resource or project. Geographic extents are described using [geojson](http://geojson.org/).

This schema references [geojson schemas](https://github.com/adiwg/mdJson-schemas/tree/master/schema/schema/geojson) defined by the ADIwg technical group for geojson feature types, and is referenced by the resourceInfo.json schema.

### [graphicOverview](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/graphicOverview.json)

The graphicOverview.json schema defines the structure of the graphic overview block of ADIwg metadata in its native JSON format. This schema defines the section of the metadata used to describe and reference images and graphics related to the data resource or project described by the metadata.

This schema is referenced by the resourceInfo.json schema.

### [keyword](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/eyword.json)

The keyword.json schema defines the structure of the keyword block of ADIwg metadata in its native JSON format. This schema defines the seciton of ADIwg metadata used to provide keywords, describe keyword types, and to provide references to authorities responsible for the controlled vocabularies used for keywords.

This schema references the citation.json schema and is referenced by the resourceInfo.json schema.

### [maintInfo](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/maintInfo)

The maintInfo.json schema defines the structure of the maintenance info block of ADIwg metadata in its native JSON format. This schema describes the structure of the objects describing the maintenance frequency of the resource, a maintenance note for providing any descriptive text about the maintenance of the resource, and for referencing the point of contact responsible for maintaining the resource.

This schema references the contact.json schema and is referenced by the metadata.json and resourceInfo.json schemas.

### [metadata](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/metadata.json)

The metadata.json schema defines the structure of the metadata block of ADIwg metadata in its native JSON format. This schema defines the structure of the main body of the metadata. This section references other schemas and describes the metadata record itself. The metadata <i>about the metadata</i> defined in this schema includes the unique identifier for the metadata record, the date of last update of the metadata, references to related metadata record(s), points of contact for metadata creation and maintenance, and the character set in which the metadata is encoded.

This schema references the citation.json, contact.json, schema.json, maintInfo.json, resourceInfo.json, and distributor.json schemas, and the MD_CharacterSetCode, DS_AssociationTypeCode, and the DS_InitiativeTypeCode codelists.

### [onlineResource](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/onlineResource.json)

The onlineResource.json schema defines the structure of the online resource block of ADIwg metadata in its native JSON format. This schema defines the metadata elements that contain names, URIs, protocol names, and text descriptions of functions performed by the online resource.

This schema references definitions from schema.json and the CI_OnlineFunctionCode codelist.

### [resolution](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/resolution.json)

The resolution.json schema defines the structure of the resolution block of ADIwg metadata in its native JSON format. This section of the metadata is used to describe the scale factor or distance for a geographic resource. Scale factor is the denominator, or x, when a map has a '1/x' scale. The distance is the ground distance measurement, including units, used to make sense of actual distances on a geographic resource and in different units. Examples of scale factor and distance are '1/100,000' and '1 in = 2.5 km', respectively.

This schema is referenced by the resourceInfo.json schema.

### [resourceConstraint](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/resourceConstraint.json)

The resourceConstraint.json schema defines the structure of the resource constraint block of ADIwg metadata in its native JSON format. This schema of the metadata is used to describe limitations on the access or use of the resource. The 'useLimitation' element allows an arbitrary string to be used to describe any general limitations or restrictions on the use of the resource; the 'legalConstraint' element provides separate sub-elements for describing legal restrictions on use and access, as well as the option to provide free-text descriptions of other constraints; and the 'securityConstraint' element provides sub-elements describing the security classification of the resource, the classification system used, any procedures that must be followed when handling or sharing the resource, and for providing notices to users explaining the legal or security prerequisites for access or use of the resource.

This schema is referenced by the resourceInfo.json schema, and references the MD_ClassificationCode and MD_RestrictionCode codelists.

### [resourceInfo](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/resourceInfo.json)

The resourceInfo.json schema defines the structure of the resource info block of ADIwg metadata in its native JSON format. This section of the metadata describes the resource itself, both directly and through reference to other json schemas describing particular aspects of the resource or the related persons and organizations.

This schema references the citation.json, extent.json, contact.json, distributor.json, keyword.json, maintInfo.json, usage.json, graphicOverview.json, resourceConstraint.json, taxonomy.json, spatialRef.json, resolution.json, and dataQuality.json schemas, and the MD_ScopeCode and MD_SpatialRepresentationTypeCode codelists.

### [taxonomy](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/taxonomy.json)

The taxonomy.json schema defines the structure of the taxonomy block of ADIwg metadata in its native JSON format. This section of the metadata is used to describe the taxa(s) included in the dataset, including keywords, taxonomic system and coverage, and the taxonomic classification systems used.

This schema references the citation.json and contact.json schemas, and is referenced by resourceInfo.json.

### [usage](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/usage)

The usage.json schema defines the structure of the usage block of ADIwg metadata in its native JSON format. This section of the metadata describes the intended and prohibited uses of the resource, and provides contact information for the the person(s) and organization(s) using the resource.

This schema references contact.json and is referenced by resourceInformation.json.
