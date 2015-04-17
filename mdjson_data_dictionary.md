# mdJSON Data DIctionary

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **additionalDocumentation**  | Additional references associated with the resource, such as: web sites, documents for additional reading, etc. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |
| resourceType  | Identifies the type of resource, such as: userGuide, website, report, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0) |
| citation  | schema for citation | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **address**  | Physical and email address at which the organization or individual may be contacted. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2) |
| deliveryPoint  | Address line for the location. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-0) |
| city  | City of the location. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-1) |
| administrativeArea  | State, province of the location. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-2) |
| postalCode  | ZIP or other postal code. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-3) |
| country  | ZIP or other postal code. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-4) |
| electronicMailAddress  | E-mail or electronic mailbox address. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-5) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **associatedResource**  | Information about a resource related to the data resource, such as: study, dataset, project, etc. An associated resource may be a child reference, or reference a larger work, such as an initiative. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| associationType  | Identifies the type of association, such as: source, cross reference, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-0) |
| initiativeType  | Identifies type of initiative under which the resource was produced - the activity that resulted in the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1) |
| resourceType  | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-2) |
| resourceCitation  | Citation for the associated resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3) |
| metadataCitation  | Citation for the associated resource metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **attribute**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7) |
| commonName  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-0) |
| codeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-1) |
| alias  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-2) |
| definition  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-3) |
| dataType  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-4) |
| allowNull  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-5) |
| units  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-6) |
| domainId  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-7) |
| minValue  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-8) |
| maxValue  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-9) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **authority**  | Citation for the authority issuing the identifier. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2) |
| title  | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-0) |
| date  | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-1) |
| responsibleParty  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-2) |
| onlineResource  | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **citation**  | Citation for the dictionary. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0) |
| edition  | Version identifier for the dictionary. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-0) |
| title  | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-0) |
| date  | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1) |
| responsibleParty  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2) |
| onlineResource  | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **classificationSystem**  | Information (citation) about the taxonomic classification system or authority used. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0) |
| edition  | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-0) |
| presentationForm  | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-1) |
| identifier  | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-2) |
| title  | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-0) |
| date  | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-1) |
| responsibleParty  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-2) |
| onlineResource  | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **constraint**  | Provides information about constraints to the use of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| useLimitation  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0) |
| legalConstraint  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1) |
| securityConstraint  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **contact**  | An array of contacts to be referenced throughout the metadata. Any contact used in the metadata record must be stored within this array and referenced by contactId. Items in array may be used 0-n times throughout the record. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1) |
| individualName  | Name of the person - surname, given name, title separated by a delimiter. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-0-0) |
| contactId  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-0) |
| positionName  | Role or position of the person, usually within a given organization. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-1) |
| address  | Physical and email address at which the organization or individual may be contacted. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2) |
| onlineResource  | Information about accessing on-line resources and services. This may be a website, profile page, GitHub page, etc. related to the contact. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-3) |
| contactInstructions  | Supplemental instructions on how or when to contact the individual or organization. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-4) |
| phoneBook  | Supplemental instructions on how or when to contact the individual or organization. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5) |
| organizationName  | Name of the organization. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-0) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **crs**  | The coordinate reference system (CRS) of a GeoJSON object. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0) |
| type  | A CRS object may link to CRS parameters on the Web. In this case, the value of its "type" member must be the string "link". | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-0) |
| properties  | An object that links to a coordinate reference system definition. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **dataDictionary**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3) |
| dictionaryInfo  | Information describing the dictionary and its source. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0) |
| domain  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1) |
| entity  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **dataQualityInfo**  | Information about the quality of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| scope  | The scope to which the data quality information is applied, for instance; dataset, attribute, feature, series, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-0) |
| lineage  | Non-quantitative quality information about the lineage of the resource as specified by the scope. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **date**  | Date referenced to the cited resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1) |
| date  | An ISO 8601 date/timestamp. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1-0-0) |
| dateType  | The type of date in the context of the citation. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **dictionaryInfo**  | Information describing the dictionary and its source. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0) |
| citation  | Citation for the dictionary. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0) |
| resourceType  | The type of resource described by the dictionary. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-1) |
| description  | Description of the dictionary. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-2) |
| language  | Language used within the dictionary. Should be a valid ISO 639-3 code. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **distributionInfo**  | Information about the distributor of and options for obtaining the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| distributorContact  | Party from whom the resource may be obtained. Note: This list need not be exhaustive. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0) |
| distributionOrderProcess  | Provides information about how the resource may be obtained and related instructions and fee information. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1) |
| distributorFormat  | Provides information about the format used by the distributor. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2) |
| distributorTransferOptions  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **distributionOrderProcess**  | Provides information about how the resource may be obtained and related instructions and fee information. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1) |
| fees  | Fees and terms for retrieving the resource, including monetary units. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-0) |
| plannedAvailabilityDateTime  | Date and time when the resource will be available. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-1) |
| orderingInstructions  | General instructions, terms and services provided by the distributor. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-2) |
| turnaround  | Typical turnaround time for the filling of an order. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **distributorContact**  | Party from whom the resource may be obtained. Note: This list need not be exhaustive. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **distributorFormat**  | Provides information about the format used by the distributor. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2) |
| formatName  | Name of the data transfer format. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2-0-0) |
| version  | Version of the format (date, number, etc.) | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **distributorTransferOptions**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |
| online  | Information about obtaining the resource on-line. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0) |
| offline  | Information about obtaining the resource through off-line procedure. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **domain**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1) |
| domainId  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-0) |
| commonName  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-1) |
| codeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-2) |
| description  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-3) |
| member  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **entity**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2) |
| entityId  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-0) |
| commonName  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-1) |
| codeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-2) |
| alias  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-3) |
| definition  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-4) |
| primaryKeyAttributeCodeName  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-5) |
| index  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6) |
| attribute  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7) |
| foreignKey  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **epsgNumber**  | The EPSG Geodetic Parameter Dataset of the reference system, see epsg-registry.org. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **extent**  | Information about the geographic extent of the resource. A resource may have multiple extents. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24) |
| description  | Description of the geographic extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-0) |
| geographicElement  | A grouping of geographic objects that comprises all or part of the extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1) |
| verticalElement  | Vertical element of an extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2) |
| temporalElement  | Temporal context for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **features**  | Set of Features constituting the FeatureCollection. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3) |
| type  | Type of GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-0) |
| geometry  | The geometry object associated with the Feature. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-1) |
| properties  | JSON object containing information about a feature or collection. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2) |
| id  | Unique identifier for the GeoJSON feature object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **foreignKey**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8) |
| localAttributeCodeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-0) |
| referencedEntityCodeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-1) |
| referencedAttributeCodeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **geographicElement**  | A grouping of geographic objects that comprises all or part of the extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1) |
| type  | Type of GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-0) |
| crs  | The coordinate reference system (CRS) of a GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0) |
| bbox  | To include information on the coordinate range for geometries, features, or feature collections, a GeoJSON object may have a member named "bbox". The value of the bbox member must be a 2*n array where n is the number of dimensions represented in the contained geometries, with the lowest values for all axes followed by the highest values. The axes order of a bbox follows the axes order of geometries. In addition, the coordinate reference system for the bbox is assumed to match the coordinate reference system of the GeoJSON object of which it is a member. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-1) |
| coordinates  | The set of Polygons that constitute the MultiPolygon. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-0-0-5-1) |
| geometries  | The set of geometry objects constituting the GeometryCollection. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-1-1) |
| geometry  | The geometry object associated with the Feature. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-2-1) |
| properties  | JSON object containing information about a feature or collection. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-1) |
| id  | Unique identifier for the GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-2) |
| features  | Set of Features constituting the FeatureCollection. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **geometries**  | The set of geometry objects constituting the GeometryCollection. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-1-1) |
| type  | Type of geometry object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-1-1-0-0-5-0) |
| coordinates  | The set of Polygons that constitute the MultiPolygon. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-1-1-0-0-5-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **geometry**  | The geometry object associated with the Feature. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-1) |
| type  | Type of geometry object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-1-0-1-0-5-0) |
| coordinates  | The set of Polygons that constitute the MultiPolygon. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-1-0-1-0-5-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **graphicOverview**  | A browse graphic associated with the resource in which to gain an at-a-glance referencing for the resource, such as geographic location and extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| fileName  | Name of the file that contains a browse graphic for the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-0) |
| fileDescription  | Description of the browse graphic. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-1) |
| fileType  | Format of the browse graphic, such as: PDF, JPEG, TIFF, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-2) |
| fileUri  | URI of the browse graphic. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **identifier**  | Identifier for the resource in the context of the citation. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2) |
| identifier  | A name that is used to identify the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-0) |
| type  | The type of identifier, e.g. doi, isbn, issn, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-1) |
| authority  | Citation for the authority issuing the identifier. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **index**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6) |
| codeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-0) |
| allowDuplicates  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-1) |
| attributeCodeName  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **keyword**  | Provides category keywords, their type, and reference source. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15) |
| keyword  | Commonly used word(s) or formalized word(s) or phrase(s) used to describe the subject. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-0) |
| keywordType  | A code, or concept, that defines the subject matter used to group similar keywords. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-1) |
| thesaurus  | Name of the formally registered thesaurus or a similar authoritative source of keywords. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **legalConstraint**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1) |
| accessConstraint  | Access constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations on obtaining the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1-0-0) |
| useConstraint  | Constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations or warnings on using the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1-0-1) |
| otherConstraint  | Other restrictions and legal prerequisites for accessing and using the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **lineage**  | Non-quantitative quality information about the lineage of the resource as specified by the scope. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1) |
| statement  | General explanation of the data producer's knowledge about the lineage of a dataset. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-0) |
| processStep  | Process or methodology steps applied to development of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-1) |
| source  | Information about the source of the resource relative to the data quality scope. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **maintenanceContact**  | Contact information for the maintainer of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **member**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4) |
| name  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-0) |
| value  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-1) |
| definition  | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **metadataCitation**  | Citation for the associated resource metadata. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4) |
| edition  | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-0) |
| presentationForm  | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-1) |
| identifier  | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-2) |
| title  | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-0) |
| date  | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-1) |
| responsibleParty  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-2) |
| onlineResource  | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **metadataContact**  | Person or organization responsible for metadata information (metadata custodian). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **metadataIdentifier**  | Unique identifier for this metadata file. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| identifier  | A name that is used to identify the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-0) |
| type  | The type of identifier, e.g. doi, isbn, issn, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-1) |
| authority  | Citation for the authority issuing the identifier. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **metadataInfo**  | General information about the metadata record. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| metadataIdentifier  | Unique identifier for this metadata file. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| parentMetadata  | Identifier of the metadata to which this metadata is a subset (child). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| metadataContact  | Person or organization responsible for metadata information (metadata custodian). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| metadataCharacterSet  | Full name of the character coding standard used for the metadata set. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3) |
| metadataCreationDate  | Date that the metadata was created. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4) |
| metadataLastUpdate  | Date that the metadata was updated. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5) |
| metadataUri  | Uniform Resource Identifier (URI) of the metadata record. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6) |
| metadataStatus  | Status of the metadata record. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7) |
| metadataMaintenance  | Provides information about the frequency of metadata updates, and the scope of those updates. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **metadataMaintenance**  | Provides information about the frequency of metadata updates, and the scope of those updates. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8) |
| maintenanceFrequency  | Describes the frequency of additions and updates made to a resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8-0) |
| maintenanceNote  | Notes regarding the maintenance of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8-1) |
| maintenanceContact  | Contact information for the maintainer of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **metadata**  | The main body of the metadata record. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2) |
| metadataInfo  | General information about the metadata record. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| resourceInfo  | Information about the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| distributionInfo  | Information about the distributor of and options for obtaining the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| associatedResource  | Information about a resource related to the data resource, such as: study, dataset, project, etc. An associated resource may be a child reference, or reference a larger work, such as an initiative. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| additionalDocumentation  | Additional references associated with the resource, such as: web sites, documents for additional reading, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **observer**  | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **offline**  | Information about obtaining the resource through off-line procedure. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1) |
| name  | Name of the format the data is distributed in, such as: dvd, hardcopy, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1-0) |
| mediumFormat  | Method used by the resource provider to write to the medium, such as: tar, iso9660, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1-1) |
| mediumNote  | Description of other limitations or requirements for using the medium. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **onlineResource**  | On-line information related to the citation. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3) |
| uri  | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-0) |
| name  | Name of the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-1) |
| protocol  | The connection protocol to be used such as: ftp, http, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-2) |
| description  | Detailed text description of what the online resource is/does. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-3) |
| function  | Function performed by the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-4) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **online**  | Information about obtaining the resource on-line. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0) |
| uri  | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-0) |
| name  | Name of the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-1) |
| protocol  | The connection protocol to be used such as: ftp, http, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-2) |
| description  | Detailed text description of what the online resource is/does. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-3) |
| function  | Function performed by the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-4) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **parentMetadata**  | Identifier of the metadata to which this metadata is a subset (child). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| edition  | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-0) |
| presentationForm  | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-1) |
| identifier  | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-2) |
| title  | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-0) |
| date  | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-1) |
| responsibleParty  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-2) |
| onlineResource  | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **phoneBook**  | Supplemental instructions on how or when to contact the individual or organization. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5) |
| phoneName  | Descriptive name of the phone number. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-0) |
| phoneNumber  | Telephone number. Recommended format is to use 'x' or 'ext' to denote extensions. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-1) |
| service  | Type(s) of phone number, e.g. voice, sms. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **pointOfContact**  | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **processStep**  | Process or methodology steps applied to the development of the source. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2) |
| stepId  | Serial identifier used to order the sequence of steps used. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-0) |
| description  | Description of the process or methodology step. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-1) |
| rationale  | Requirement or purpose for the process or methodology step. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-2) |
| dateTime  | Date and time or date at which the process or methodology step occurred. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-3) |
| processor  | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **processor**  | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **properties**  | JSON object containing information about a feature or collection. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2) |
| includesData  | A boolean indicating whether geographic object is defining an extent, or used to describe an area of exception, such as "holes" in polygons. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-0) |
| temporalElement  | The temporal reference associated with an feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-1) |
| verticalElement  | The vertical extent of the feature geometry. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-2) |
| description  | A description of the feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-3) |
| featureName  | A title associated with a feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-4) |
| featureScope  | Scope of the geographic feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-5) |
| featureAcquisitionMethod  | Method used to establish the position of the geographic feature.  | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-6) |
| identifier  | Identifier for the geographic element with optional cited authority. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-7) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **properties**  | An object that links to a coordinate reference system definition. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-1) |
| href  | A dereferenceable URI that links to the parameters for the coordinate reference system. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-1-0) |
| type  | A string that hints at the format used to represent CRS parameters at the provided URI. Suggested values are: "proj4", "ogcwkt", "esriwkt", but others can be used. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-1-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **repository**  | Information about the curator or contact person and/or agency responsible for the specimens. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **resourceCitation**  | Citation for the associated resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3) |
| edition  | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-0) |
| presentationForm  | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-1) |
| identifier  | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-2) |
| title  | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-0) |
| date  | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-1) |
| responsibleParty  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-2) |
| onlineResource  | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **resourceInfo**  | Information about the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| resourceType  | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-0) |
| citation  | Citation for the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-1) |
| resourceTimePeriod  | Time period for the resource, e.g. project start and end date(s). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2) |
| pointOfContact  | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3) |
| abstract  | Brief narrative summary of the content of the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-4) |
| shortAbstract  | A short description of the resource. Max of 300 characters. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-5) |
| status  | Status of the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-6) |
| hasMapLocation  | A flag indicating that a resource has a geographic location associated with it and therefore can be located using a map interface. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-7) |
| hasDataAvailable  | A flag to indicate whether data for this resource is available for distribution. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-8) |
| language  | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9) |
| purpose  | A summary of intentions for which the resource was created. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-10) |
| credit  | A narrative identification of additional resources credited for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11) |
| topicCategory  | General theme keyword of the resource, such as: oceans, biota atmosphere, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12) |
| environmentDescription  | Description of the dataset in the producer's processing environment, including items such as the software, the computer, the computer operating system, file name, and the dataset size. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13) |
| resourceNativeFormat  | Provides a description of the format of the resource(s). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14) |
| keyword  | Provides category keywords, their type, and reference source. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15) |
| resourceMaintenance  | Information about the maintenance of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| resourceSpecificUsage  | Description of ways in which the resource is currently or has been used. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| graphicOverview  | A browse graphic associated with the resource in which to gain an at-a-glance referencing for the resource, such as geographic location and extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| constraint  | Provides information about constraints to the use of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| taxonomy  | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20) |
| spatialReferenceSystem  | Geospatial referencing system associated with describing the geospatial extent of the data resource. The referencing can be provided indirectly by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| spatialRepresentation  | Format of the resource geographic extent, such as: vector, grid, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22) |
| spatialResolution  | Information about the scale of the geographic extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| extent  | Information about the geographic extent of the resource. A resource may have multiple extents. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24) |
| dataQualityInfo  | Information about the quality of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| supplementalInfo  | Any other descriptive information about the dataset. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **resourceMaintenance**  | Information about the maintenance of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| maintenanceFrequency  | Describes the frequency of additions and updates made to a resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-0) |
| maintenanceNote  | Notes regarding the maintenance of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-1) |
| maintenanceContact  | Contact information for the maintainer of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **resourceNativeFormat**  | Provides a description of the format of the resource(s). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14) |
| formatName  | Name of the data transfer format. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-0) |
| version  | Version of the format (date, number, etc.) | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **resourceSpecificUsage**  | Description of ways in which the resource is currently or has been used. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| specificUsage  | Brief description of the resource usage. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-0) |
| userDeterminedLimitation  | Usage that the provider's have determined the resource not being suitable for. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-1) |
| userContactInfo  | Identification of and means of communicating with the person(s) and organization(s) using the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **resourceTimePeriod**  | Time period for the resource, e.g. project start and end date(s). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2) |
| id  | A unique identifier for a temporal element. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-0) |
| description  | Text associated with the time instance. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-1) |
| beginPosition  | Starting date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-2) |
| endPosition  | Ending date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **responsibleParty**  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **schema**  | schema for ADIwg mdJSON metadata |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=) |
| version  | Identifies the version of the JSON schema standard that applies to the metadata. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0) |
| contact  | An array of contacts to be referenced throughout the metadata. Any contact used in the metadata record must be stored within this array and referenced by contactId. Items in array may be used 0-n times throughout the record. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1) |
| metadata  | The main body of the metadata record. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2) |
| dataDictionary  | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **securityConstraint**  | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2) |
| classification  | Name of the handling restrictions on the resource or metadata. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-0) |
| userNote  | Explanation of the application of the legal constraints or other restrictions and legal prerequisites for obtaining and using the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-1) |
| classificationSystem  | Name of the classification system associated with a security constraint. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-2) |
| handlingDescription  | Additional description regarding the security handling of the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **source**  | Information about the source of the resource relative to the data quality scope. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2) |
| description  | Description of the source for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-0) |
| citation  | Citation for the source. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-1) |
| processStep  | Process or methodology steps applied to the development of the source. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **spatialReferenceSystem**  | Geospatial referencing system associated with describing the geospatial extent of the data resource. The referencing can be provided indirectly by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| name  | A recognized reference system name. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0) |
| epsgNumber  | The EPSG Geodetic Parameter Dataset of the reference system, see epsg-registry.org. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1) |
| wkt  | Well-known text representation of the reference system. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **spatialResolution**  | Information about the scale of the geographic extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| equivalentScale  | Scale of geographic extent expressed in a hardcopy map scale fraction (denominator). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0-0-0) |
| distance  | Ground distance measurement representing geographic extent. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0-1-0) |
| uom  | Ground distance units of measure. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0-1-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **taxonClass**  | Information about the range of taxa addressed in the data set or collection. It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division/Phylum, class, Order, Family, Genus, and Species should be included as ranks as appropriate. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5) |
| taxonRank  | Name of the taxonomic rank for which the taxonValue is provided. Example: "Kingdom", "Division", "Phylum", "Subphylum", "SuperClass", "Class", "SubClass", "InfraClass", "Superorder", "Order", "Suborder", "Infraorder", "Superfamily", "Family", "Subfamily", "Tribe", "Subtribe", "Genus", "Species". | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5-0-0) |
| taxonValue  | Taxonomic rank value of the taxon being described. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5-0-1) |
| common  | Specification of applicable common names. These common names may be general descriptions of a group of organisms if appropriate (e.g. insects, vertebrate, grasses, waterfowl, vascular plants, etc.). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **taxonomy**  | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20) |
| classificationSystem  | Information (citation) about the taxonomic classification system or authority used. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0) |
| taxonGeneralScope  | Description of the range of taxa addressed in the data set or collection. For example, "all vascular plants were identified to family or species, mosses and lichens were identified as moss or lichen". | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-1) |
| observer  | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2) |
| taxonomicProcedure  | Description of the methods used for taxonomic identification. Could include specimen processing, comparison with museum materials, keys, and key characters, chemical or genetic analyses, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-3) |
| voucher  | Information on the types of specimen, the repository, and the individuals who identified the vouchers. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4) |
| taxonClass  | Information about the range of taxa addressed in the data set or collection. It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division/Phylum, class, Order, Family, Genus, and Species should be included as ranks as appropriate. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **temporalElement**  | Temporal context for the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3) |
| timeInstant  | A set of date time instances. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0) |
| timePeriod  | A set of time periods. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1) |
| date  | A set of date times. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **thesaurus**  | Name of the formally registered thesaurus or a similar authoritative source of keywords. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2) |
| edition  | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-0) |
| presentationForm  | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-1) |
| identifier  | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-2) |
| title  | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-0) |
| date  | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-1) |
| responsibleParty  | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-2) |
| onlineResource  | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **timeInstant**  | A set of date time instances. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0) |
| id  | A unique identifier for a temporal element. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0-0-0) |
| description  | Text associated with the time instance. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0-0-1) |
| timePosition  | An ISO 8601 date/timestamp. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0-0-2) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **timePeriod**  | A set of time periods. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1) |
| id  | A unique identifier for a temporal element. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-0) |
| description  | Text associated with the time instance. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-1) |
| beginPosition  | Starting date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-2) |
| endPosition  | Ending date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **userContactInfo**  | Identification of and means of communicating with the person(s) and organization(s) using the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2) |
| contactId  | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-0-0) |
| role  | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **version**  | Identifies the version of the JSON schema standard that applies to the metadata. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0) |
| name  | Schema identifier, i.e. the name of the schema standard. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-0) |
| version  | Specific version number of the schema standard. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-1) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **verticalElement**  | Vertical element of an extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2) |
| minimumValue  | Lowest vertical extent contained in the dataset. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-0) |
| maximumValue  | Highest vertical extent contained in the dataset. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-1) |
| verticalCRSTitle  | Name of a geographic reference system associated with a vertical extent. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-2) |
| verticalCRSUri  | Web link to the parameters for a geographic reference system associated with a vertical extent. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-3) |

| Name  | Description | Required | Viewer Link|
|---|---|---|---|
| **voucher**  | Information on the types of specimen, the repository, and the individuals who identified the vouchers. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4) |
| specimen  | Word or phrase describing the type of specimen collected (e.g. herbarium specimens, blood samples, photographs, individuals, or batches). Example: "herbarium specimens", "blood samples", "photographs", "individuals", "free text". | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-0) |
| repository  | Information about the curator or contact person and/or agency responsible for the specimens. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1) |