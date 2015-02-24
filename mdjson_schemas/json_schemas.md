#
# JSON Schemas

### [citation](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/citation.json)

The citation.json schema file defines the structure of the citation block of ADIwg metadata in its native JSON format. This section of the metadata is used to reference a published or unpublished data and information products about the data or effort described by the metadata record. Uses of the citation schema in ADIwg metadata typically include one or more citations for the dataset or sampling effort described by the metadata; references to authorities responsible for any taxonomies or controlled vocabularies used in the metadata; and to provide a reference to a data or processing-step source in the dataset lineage.

The citation schema is referenced by the dataQuality, keyword, metadata, and  taxonomy schemas. This schema references the contact schema defined below.

### [contact](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/contact.json)

The contact.json schema defines the structure of the contact block of ADIwg metadata in its native JSON format. This section of the metadata is used to provide credit to the individuals and organizations responsible for funding,
collecting, processing, managing, or preserving the data during some part of the data lifecycle. For each individual or organization listed as a contact, this schema defines the metadata elements describing the names, physical and email addresses, position titles, phone numbers and types, online resource information and formats, and the role of each contact in the data lifecycle.

The contact.json schema is directly referenced by the citation, dataQuality, distibutor, metadata, maintInfo, resourceInfo, taxonomy, and usage JSON schemas.

### [dataQuality](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/dataQuality.json)

The dataQuality.json schema defines the structure of the data quality block of ADIwg metadata in its native JSON format. This section of the metadata describes the lineage of the project or data resource decribed by the metadata record. This history of the resource is modeled in terms of process steps and sources. Process steps provide elements describing a rationale, narrative description, process date, and processor point of contact elements. Sources are described with a narrative description, a reference to a citation block describing the source or a metadata record describing the source, and a reference to a process step performed on the source.

The dataQuality schema is referenced by resourceInfo.json. This schema references the citation and contact schemas.

### [distibutor](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/distributor.json)

The distributor.json schema defines the structure of the distributor block of ADIwg metadata in its native JSON format. The distributor block provides information on the means of delivery available for the resource, the formats in which the resource is available, and references the points of contact for the distributors of the resource.

This schema references the contact.json and onlineResource.json schemas, and is referenced by the metadata.json and resourceInfo.json schemas.

### [extent](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/extent.json)

The extent.json schema defines the structure of the extent block of ADIwg metadata in its native JSON format. The extent block describes the spatial regions and time periods that are relevant to the areas and periods of data collection and the descriptive breadth of the resource or project. Geographic extents are described using [geojson](http://geojson.org/).

This schema references [geojson schemas](https://github.com/adiwg/mdJson-schemas/tree/master/schema/schema/geojson) defined by the ADIwg technical group for geojson feature types, and is referenced by the resourceInfo.json schema.

### [graphicOverview](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/graphicOverview.json)

The graphicOverview.json schema defines the structure of the graphic overview block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [keyword](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/eyword.json)

The keyword.json schema defines the structure of the keyword block of ADIwg metadata in its native JSON format. This schema defines the seciton of ADIwg metadata used to provide keywords, describe keyword types, and to provide references to authorities responsible for the controlled vocaularies used for keywords.

This schema references the citation.json schema and is referenced by the resourceInfo.json schema.

### [maintInfo](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/maintInfo)

The maintInfo.json schema defines the structure of the maintenance info block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [metadata](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/metadata.json)

The metadata.json schema defines the structure of the metadata block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [onlineResource](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/onlineResource.json)

The onlineResource.json schema defines the structure of the online resource block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [resolution](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/resolution.json)

The resolution.json schema defines the structure of the resolution block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [resourceConstraint](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/resourceConstraint.json)

The resourceConstraint.json schema defines the structure of the resource constraint block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [resourceInfo](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/resourceInfo.json)

The resourceInfo.json schema defines the structure of the resource info block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [taxonomy](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/taxonomy.json)

The taxonomy.json schema defines the structure of the taxonomy block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...

### [usage](https://github.com/adiwg/mdJson-schemas/blob/master/schema/schema/usage)

The usage.json schema defines the structure of the usage block of ADIwg metadata in its native JSON format.

This section of the metadata is used to reference ...

This schema references the ...
