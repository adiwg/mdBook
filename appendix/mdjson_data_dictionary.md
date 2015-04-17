# mdJSON Data Dictionary

<!-- toc -->

##additionalDocumentation
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **additionalDocumentation** | array | Additional references associated with the resource, such as: web sites, documents for additional reading, etc. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |
| resourceType |string | Identifies the type of resource, such as: userGuide, website, report, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0) |
| citation |object | schema for citation | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1) |

##address
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **address** | object | Physical and email address at which the organization or individual may be contacted. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2) |
| deliveryPoint |array | Address line for the location. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-0) |
| city |string | City of the location. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-1) |
| administrativeArea |string | State, province of the location. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-2) |
| postalCode |string | ZIP or other postal code. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-3) |
| country |string | ZIP or other postal code. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-4) |
| electronicMailAddress |array | E-mail or electronic mailbox address. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-5) |

##associatedResource
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **associatedResource** | array | Information about a resource related to the data resource, such as: study, dataset, project, etc. An associated resource may be a child reference, or reference a larger work, such as an initiative. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| associationType |string | Identifies the type of association, such as: source, cross reference, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-0) |
| initiativeType |string | Identifies type of initiative under which the resource was produced - the activity that resulted in the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1) |
| resourceType |string | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-2) |
| resourceCitation |object | Citation for the associated resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3) |
| metadataCitation |object | Citation for the associated resource metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4) |

##attribute
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **attribute** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7) |
| commonName |string | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-0) |
| codeName |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-1) |
| alias |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-2) |
| definition |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-3) |
| dataType |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-4) |
| allowNull |boolean | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-5) |
| units |string | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-6) |
| domainId |string | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-7) |
| minValue |string | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-8) |
| maxValue |string | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-9) |

##authority
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **authority** | object | Citation for the authority issuing the identifier. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2) |
| title |string | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-0) |
| date |array | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-1) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-2) |
| onlineResource |array | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2-3) |

##citation
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **citation** | object | Citation for the dictionary. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0) |
| edition |string | Version identifier for the dictionary. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-0) |
| title |string | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-0) |
| date |array | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2) |
| onlineResource |array | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3) |

##classificationSystem
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **classificationSystem** | array | Information (citation) about the taxonomic classification system or authority used. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0) |
| edition |string | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-2) |
| title |string | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-0) |
| date |array | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-1) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-2) |
| onlineResource |array | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0-0-0-3-0-3) |

##constraint
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **constraint** | object | Provides information about constraints to the use of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| useLimitation |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0) |
| legalConstraint |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1) |
| securityConstraint |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2) |

##contact
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **contact** | array | An array of contacts to be referenced throughout the metadata. Any contact used in the metadata record must be stored within this array and referenced by contactId. Items in array may be used 0-n times throughout the record. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1) |
| individualName |string | Name of the person - surname, given name, title separated by a delimiter. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-0-0) |
| contactId |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-0) |
| positionName |string | Role or position of the person, usually within a given organization. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-1) |
| address |object | Physical and email address at which the organization or individual may be contacted. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2) |
| onlineResource |array | Information about accessing on-line resources and services. This may be a website, profile page, GitHub page, etc. related to the contact. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-3) |
| contactInstructions |string | Supplemental instructions on how or when to contact the individual or organization. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-4) |
| phoneBook |array | Supplemental instructions on how or when to contact the individual or organization. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5) |
| organizationName |string | Name of the organization. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-0) |

##dataDictionary
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **dataDictionary** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3) |
| dictionaryInfo |object | Information describing the dictionary and its source. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0) |
| domain |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1) |
| entity |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2) |

##dataQualityInfo
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **dataQualityInfo** | array | Information about the quality of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| scope |string | The scope to which the data quality information is applied, for instance; dataset, attribute, feature, series, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-0) |
| lineage |object | Non-quantitative quality information about the lineage of the resource as specified by the scope. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1) |

##date
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **date** | array | Date referenced to the cited resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1) |
| date |string | An ISO 8601 date/timestamp. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1-0-0) |
| dateType |string | The type of date in the context of the citation. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1-0-1) |

##dictionaryInfo
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **dictionaryInfo** | object | Information describing the dictionary and its source. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0) |
| citation |object | Citation for the dictionary. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0) |
| resourceType |string | The type of resource described by the dictionary. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-1) |
| description |string | Description of the dictionary. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-2) |
| language |string | Language used within the dictionary. Should be a valid ISO 639-3 code. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-3) |

##distributionInfo
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **distributionInfo** | array | Information about the distributor of and options for obtaining the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| distributorContact |object | Party from whom the resource may be obtained. Note: This list need not be exhaustive. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0) |
| distributionOrderProcess |array | Provides information about how the resource may be obtained and related instructions and fee information. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1) |
| distributorFormat |array | Provides information about the format used by the distributor. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2) |
| distributorTransferOptions |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |

##distributionOrderProcess
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **distributionOrderProcess** | array | Provides information about how the resource may be obtained and related instructions and fee information. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1) |
| fees |string | Fees and terms for retrieving the resource, including monetary units. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-0) |
| plannedAvailabilityDateTime |string | Date and time when the resource will be available. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-1) |
| orderingInstructions |string | General instructions, terms and services provided by the distributor. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-2) |
| turnaround |string | Typical turnaround time for the filling of an order. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-3) |

##distributorContact
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **distributorContact** | object | Party from whom the resource may be obtained. Note: This list need not be exhaustive. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0-1) |

##distributorFormat
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **distributorFormat** | array | Provides information about the format used by the distributor. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2) |
| formatName |string | Name of the data transfer format. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2-0-0) |
| version |string | Version of the format (date, number, etc.) | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2-0-1) |

##distributorTransferOptions
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **distributorTransferOptions** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |
| online |array | Information about obtaining the resource on-line. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0) |
| offline |object | Information about obtaining the resource through off-line procedure. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1) |

##domain
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **domain** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1) |
| domainId |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-0) |
| commonName |string | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-1) |
| codeName |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-2) |
| description |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-3) |
| member |array | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4) |

##entity
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **entity** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2) |
| entityId |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-0) |
| commonName |string | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-1) |
| codeName |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-2) |
| alias |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-3) |
| definition |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-4) |
| primaryKeyAttributeCodeName |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-5) |
| index |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6) |
| attribute |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7) |
| foreignKey |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8) |

##epsgNumber
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **epsgNumber** | array | The EPSG Geodetic Parameter Dataset of the reference system, see epsg-registry.org. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1) |

##extent
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **extent** | array | Information about the geographic extent of the resource. A resource may have multiple extents. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24) |
| description |string | Description of the geographic extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-0) |
| geographicElement |array | A grouping of geographic objects that comprises all or part of the extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1) |
| verticalElement |array | Vertical element of an extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2) |
| temporalElement |object | Temporal context for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3) |

##features
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **features** | array | Set of Features constituting the FeatureCollection. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3) |
| type |enum: Feature | Type of GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-0) |
| geometry |ambiguous | The geometry object associated with the Feature. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-1) |
| properties |ambiguous | JSON object containing information about a feature or collection. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2) |
| id |string,number | Unique identifier for the GeoJSON feature object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-3) |

##foreignKey
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **foreignKey** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8) |
| localAttributeCodeName |array | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-0) |
| referencedEntityCodeName |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-1) |
| referencedAttributeCodeName |array | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-2) |

##geographicElement
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **geographicElement** | array | A grouping of geographic objects that comprises all or part of the extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1) |
| type |enum: FeatureCollection | Type of GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-0) |
| crs |ambiguous | The coordinate reference system (CRS) of a GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0) |
| bbox |array | To include information on the coordinate range for geometries, features, or feature collections, a GeoJSON object may have a member named "bbox". The value of the bbox member must be a 2*n array where n is the number of dimensions represented in the contained geometries, with the lowest values for all axes followed by the highest values. The axes order of a bbox follows the axes order of geometries. In addition, the coordinate reference system for the bbox is assumed to match the coordinate reference system of the GeoJSON object of which it is a member. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-1) |
| coordinates |array | The set of Polygons that constitute the MultiPolygon. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-0-0-5-1) |
| geometries |array | The set of geometry objects constituting the GeometryCollection. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-1-1) |
| geometry |ambiguous | The geometry object associated with the Feature. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-2-1) |
| properties |ambiguous | JSON object containing information about a feature or collection. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-1) |
| id |string,number | Unique identifier for the GeoJSON object. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-2) |
| features |array | Set of Features constituting the FeatureCollection. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3) |

##graphicOverview
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **graphicOverview** | array | A browse graphic associated with the resource in which to gain an at-a-glance referencing for the resource, such as geographic location and extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| fileName |string | Name of the file that contains a browse graphic for the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-0) |
| fileDescription |string | Description of the browse graphic. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-1) |
| fileType |string | Format of the browse graphic, such as: PDF, JPEG, TIFF, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-2) |
| fileUri |string | URI of the browse graphic. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-3) |

##identifier
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **identifier** | array | Identifier for the resource in the context of the citation. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2) |
| identifier |string | A name that is used to identify the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-0) |
| type |string | The type of identifier, e.g. doi, isbn, issn, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-1) |
| authority |object | Citation for the authority issuing the identifier. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2) |

##index
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **index** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6) |
| codeName |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-0) |
| allowDuplicates |boolean | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-1) |
| attributeCodeName |array | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-2) |

##keyword
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **keyword** | array | Provides category keywords, their type, and reference source. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15) |
| keyword |array | Commonly used word(s) or formalized word(s) or phrase(s) used to describe the subject. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-0) |
| keywordType |string | A code, or concept, that defines the subject matter used to group similar keywords. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-1) |
| thesaurus |object | Name of the formally registered thesaurus or a similar authoritative source of keywords. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2) |

##legalConstraint
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **legalConstraint** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1) |
| accessConstraint |array | Access constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations on obtaining the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1-0-0) |
| useConstraint |array | Constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations or warnings on using the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1-0-1) |
| otherConstraint |array | Other restrictions and legal prerequisites for accessing and using the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-1-0-2) |

##lineage
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **lineage** | object | Non-quantitative quality information about the lineage of the resource as specified by the scope. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1) |
| statement |string | General explanation of the data producer's knowledge about the lineage of a dataset. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-0) |
| processStep |array | Process or methodology steps applied to development of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-1) |
| source |array | Information about the source of the resource relative to the data quality scope. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2) |

##maintenanceContact
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **maintenanceContact** | array | Contact information for the maintainer of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-0-1) |

##member
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **member** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4) |
| name |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-0) |
| value |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-1) |
| definition |string | undefined | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-2) |

##metadataCitation
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **metadataCitation** | object | Citation for the associated resource metadata. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4) |
| edition |string | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-2) |
| title |string | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-0) |
| date |array | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-1) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-2) |
| onlineResource |array | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-3) |

##metadataContact
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **metadataContact** | array | Person or organization responsible for metadata information (metadata custodian). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-0-1) |

##metadataIdentifier
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **metadataIdentifier** | object | Unique identifier for this metadata file. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| identifier |string | A name that is used to identify the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-0) |
| type |string | The type of identifier, e.g. doi, isbn, issn, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-1) |
| authority |object | Citation for the authority issuing the identifier. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-2) |

##metadataInfo
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **metadataInfo** | object | General information about the metadata record. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| metadataIdentifier |object | Unique identifier for this metadata file. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| parentMetadata |object | Identifier of the metadata to which this metadata is a subset (child). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| metadataContact |array | Person or organization responsible for metadata information (metadata custodian). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| metadataCharacterSet |string | Full name of the character coding standard used for the metadata set. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3) |
| metadataCreationDate |string | Date that the metadata was created. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4) |
| metadataLastUpdate |string | Date that the metadata was updated. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5) |
| metadataUri |string | Uniform Resource Identifier (URI) of the metadata record. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6) |
| metadataStatus |string | Status of the metadata record. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7) |
| metadataMaintenance |object | Provides information about the frequency of metadata updates, and the scope of those updates. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8) |

##metadataMaintenance
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **metadataMaintenance** | object | Provides information about the frequency of metadata updates, and the scope of those updates. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8) |
| maintenanceFrequency |string | Describes the frequency of additions and updates made to a resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8-0) |
| maintenanceNote |array | Notes regarding the maintenance of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8-1) |
| maintenanceContact |array | Contact information for the maintainer of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8-2) |

##metadata
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **metadata** | object | The main body of the metadata record. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2) |
| metadataInfo |object | General information about the metadata record. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| resourceInfo |object | Information about the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| distributionInfo |array | Information about the distributor of and options for obtaining the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| associatedResource |array | Information about a resource related to the data resource, such as: study, dataset, project, etc. An associated resource may be a child reference, or reference a larger work, such as an initiative. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| additionalDocumentation |array | Additional references associated with the resource, such as: web sites, documents for additional reading, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |

##observer
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **observer** | array | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2-0-1) |

##offline
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **offline** | object | Information about obtaining the resource through off-line procedure. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1) |
| name |string | Name of the format the data is distributed in, such as: dvd, hardcopy, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1-0) |
| mediumFormat |string | Method used by the resource provider to write to the medium, such as: tar, iso9660, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1-1) |
| mediumNote |string | Description of other limitations or requirements for using the medium. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1-2) |

##onlineResource
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **onlineResource** | array | On-line information related to the citation. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-0) |
| name |string | Name of the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-3) |
| function |string | Function performed by the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-4) |

##online
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **online** | array | Information about obtaining the resource on-line. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-0) |
| name |string | Name of the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-3) |
| function |string | Function performed by the online resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-4) |

##parentMetadata
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **parentMetadata** | object | Identifier of the metadata to which this metadata is a subset (child). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| edition |string | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-2) |
| title |string | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-0) |
| date |array | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-1) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-2) |
| onlineResource |array | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-3) |

##phoneBook
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **phoneBook** | array | Supplemental instructions on how or when to contact the individual or organization. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5) |
| phoneName |string | Descriptive name of the phone number. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-0) |
| phoneNumber |string | Telephone number. Recommended format is to use 'x' or 'ext' to denote extensions. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-1) |
| service |array | Type(s) of phone number, e.g. voice, sms. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-2) |

##pointOfContact
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **pointOfContact** | array | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3-0-1) |

##processStep
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **processStep** | array | Process or methodology steps applied to the development of the source. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2) |
| stepId |string | Serial identifier used to order the sequence of steps used. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-0) |
| description |string | Description of the process or methodology step. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-1) |
| rationale |string | Requirement or purpose for the process or methodology step. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-2) |
| dateTime |string | Date and time or date at which the process or methodology step occurred. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-3) |
| processor |array | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4) |

##processor
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **processor** | array | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2-0-4-0-1) |

##properties
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **properties** | ambiguous | JSON object containing information about a feature or collection. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2) |
| includesData |boolean | A boolean indicating whether geographic object is defining an extent, or used to describe an area of exception, such as "holes" in polygons. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-0) |
| temporalElement |object | The temporal reference associated with an feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-1) |
| verticalElement |array | The vertical extent of the feature geometry. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-2) |
| description |string | A description of the feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-3) |
| featureName |string | A title associated with a feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-4) |
| featureScope |string | Scope of the geographic feature. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-5) |
| featureAcquisitionMethod |string | Method used to establish the position of the geographic feature.  | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-6) |
| identifier |array | Identifier for the geographic element with optional cited authority. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-2-3-3-0-2-0-1-7) |

##properties
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **properties** | object | An object that links to a coordinate reference system definition. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-1) |
| href |string | A dereferenceable URI that links to the parameters for the coordinate reference system. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-1-0) |
| type |string | A string that hints at the format used to represent CRS parameters at the provided URI. Suggested values are: "proj4", "ogcwkt", "esriwkt", but others can be used. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1-0-1-0-0-0-0-2-1-1-1) |

##repository
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **repository** | object | Information about the curator or contact person and/or agency responsible for the specimens. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1-1) |

##resourceCitation
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **resourceCitation** | object | Citation for the associated resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3) |
| edition |string | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-2) |
| title |string | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-0) |
| date |array | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-1) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-2) |
| onlineResource |array | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-3) |

##resourceInfo
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **resourceInfo** | object | Information about the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| resourceType |string | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-0) |
| citation |object | Citation for the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-1) |
| resourceTimePeriod |object | Time period for the resource, e.g. project start and end date(s). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2) |
| pointOfContact |array | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3) |
| abstract |string | Brief narrative summary of the content of the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-4) |
| shortAbstract |string | A short description of the resource. Max of 300 characters. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-5) |
| status |string | Status of the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-6) |
| hasMapLocation |boolean | A flag indicating that a resource has a geographic location associated with it and therefore can be located using a map interface. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-7) |
| hasDataAvailable |boolean | A flag to indicate whether data for this resource is available for distribution. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-8) |
| language |array | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9) |
| purpose |string | A summary of intentions for which the resource was created. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-10) |
| credit |array | A narrative identification of additional resources credited for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11) |
| topicCategory |array | General theme keyword of the resource, such as: oceans, biota atmosphere, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12) |
| environmentDescription |string | Description of the dataset in the producer's processing environment, including items such as the software, the computer, the computer operating system, file name, and the dataset size. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13) |
| resourceNativeFormat |array | Provides a description of the format of the resource(s). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14) |
| keyword |array | Provides category keywords, their type, and reference source. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15) |
| resourceMaintenance |array | Information about the maintenance of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| resourceSpecificUsage |array | Description of ways in which the resource is currently or has been used. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| graphicOverview |array | A browse graphic associated with the resource in which to gain an at-a-glance referencing for the resource, such as geographic location and extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| constraint |object | Provides information about constraints to the use of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| taxonomy |object | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20) |
| spatialReferenceSystem |object | Geospatial referencing system associated with describing the geospatial extent of the data resource. The referencing can be provided indirectly by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| spatialRepresentation |array | Format of the resource geographic extent, such as: vector, grid, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22) |
| spatialResolution |array | Information about the scale of the geographic extent. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| extent |array | Information about the geographic extent of the resource. A resource may have multiple extents. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24) |
| dataQualityInfo |array | Information about the quality of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| supplementalInfo |string | Any other descriptive information about the dataset. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26) |

##resourceMaintenance
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **resourceMaintenance** | array | Information about the maintenance of the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| maintenanceFrequency |string | Describes the frequency of additions and updates made to a resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-0) |
| maintenanceNote |array | Notes regarding the maintenance of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-1) |
| maintenanceContact |array | Contact information for the maintainer of the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2) |

##resourceNativeFormat
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **resourceNativeFormat** | array | Provides a description of the format of the resource(s). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14) |
| formatName |string | Name of the data transfer format. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-0) |
| version |string | Version of the format (date, number, etc.) | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-1) |

##resourceSpecificUsage
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **resourceSpecificUsage** | array | Description of ways in which the resource is currently or has been used. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| specificUsage |string | Brief description of the resource usage. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-0) |
| userDeterminedLimitation |string | Usage that the provider's have determined the resource not being suitable for. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-1) |
| userContactInfo |array | Identification of and means of communicating with the person(s) and organization(s) using the resource. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2) |

##resourceTimePeriod
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **resourceTimePeriod** | object | Time period for the resource, e.g. project start and end date(s). |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2) |
| id |string | A unique identifier for a temporal element. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-0) |
| description |string | Text associated with the time instance. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-1) |
| beginPosition |string | Starting date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-2) |
| endPosition |string | Ending date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-3) |

##responsibleParty
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **responsibleParty** | array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2-0-1) |

##schema
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **schema** | object | schema for ADIwg mdJSON metadata |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=) |
| version |object | Identifies the version of the JSON schema standard that applies to the metadata. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0) |
| contact |array | An array of contacts to be referenced throughout the metadata. Any contact used in the metadata record must be stored within this array and referenced by contactId. Items in array may be used 0-n times throughout the record. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1) |
| metadata |object | The main body of the metadata record. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2) |
| dataDictionary |array | undefined | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3) |

##securityConstraint
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **securityConstraint** | array | undefined |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2) |
| classification |string | Name of the handling restrictions on the resource or metadata. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-0) |
| userNote |string | Explanation of the application of the legal constraints or other restrictions and legal prerequisites for obtaining and using the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-1) |
| classificationSystem |string | Name of the classification system associated with a security constraint. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-2) |
| handlingDescription |string | Additional description regarding the security handling of the resource or metadata. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-2-0-3) |

##source
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **source** | array | Information about the source of the resource relative to the data quality scope. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2) |
| description |string | Description of the source for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-0) |
| citation |object | Citation for the source. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-1) |
| processStep |array | Process or methodology steps applied to the development of the source. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-2-0-2) |

##spatialReferenceSystem
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **spatialReferenceSystem** | object | Geospatial referencing system associated with describing the geospatial extent of the data resource. The referencing can be provided indirectly by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| name |array | A recognized reference system name. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0) |
| epsgNumber |array | The EPSG Geodetic Parameter Dataset of the reference system, see epsg-registry.org. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1) |
| wkt |array | Well-known text representation of the reference system. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2) |

##spatialResolution
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **spatialResolution** | array | Information about the scale of the geographic extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| equivalentScale |number | Scale of geographic extent expressed in a hardcopy map scale fraction (denominator). | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0-0-0) |
| distance |number | Ground distance measurement representing geographic extent. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0-1-0) |
| uom |string | Ground distance units of measure. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0-1-1) |

##taxonClass
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **taxonClass** | array | Information about the range of taxa addressed in the data set or collection. It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division/Phylum, class, Order, Family, Genus, and Species should be included as ranks as appropriate. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5) |
| taxonRank |string | Name of the taxonomic rank for which the taxonValue is provided. Example: "Kingdom", "Division", "Phylum", "Subphylum", "SuperClass", "Class", "SubClass", "InfraClass", "Superorder", "Order", "Suborder", "Infraorder", "Superfamily", "Family", "Subfamily", "Tribe", "Subtribe", "Genus", "Species". | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5-0-0) |
| taxonValue |string | Taxonomic rank value of the taxon being described. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5-0-1) |
| common |string | Specification of applicable common names. These common names may be general descriptions of a group of organisms if appropriate (e.g. insects, vertebrate, grasses, waterfowl, vascular plants, etc.). | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5-0-2) |

##taxonomy
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **taxonomy** | object | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20) |
| classificationSystem |array | Information (citation) about the taxonomic classification system or authority used. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0) |
| taxonGeneralScope |string | Description of the range of taxa addressed in the data set or collection. For example, "all vascular plants were identified to family or species, mosses and lichens were identified as moss or lichen". | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-1) |
| observer |array | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-2) |
| taxonomicProcedure |string | Description of the methods used for taxonomic identification. Could include specimen processing, comparison with museum materials, keys, and key characters, chemical or genetic analyses, etc. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-3) |
| voucher |object | Information on the types of specimen, the repository, and the individuals who identified the vouchers. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4) |
| taxonClass |array | Information about the range of taxa addressed in the data set or collection. It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division/Phylum, class, Order, Family, Genus, and Species should be included as ranks as appropriate. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-5) |

##temporalElement
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **temporalElement** | object | Temporal context for the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3) |
| timeInstant |array | A set of date time instances. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0) |
| timePeriod |array | A set of time periods. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1) |
| date |array | A set of date times. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-2) |

##thesaurus
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **thesaurus** | object | Name of the formally registered thesaurus or a similar authoritative source of keywords. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2) |
| edition |string | Version identifier for the resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-2) |
| title |string | Name by which the cited resource is known. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-0) |
| date |array | Date referenced to the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-1) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-2) |
| onlineResource |array | On-line information related to the citation. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2-3-0-3) |

##timeInstant
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **timeInstant** | array | A set of date time instances. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0) |
| id |string | A unique identifier for a temporal element. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0-0-0) |
| description |string | Text associated with the time instance. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0-0-1) |
| timePosition |string | An ISO 8601 date/timestamp. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-0-0-2) |

##timePeriod
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **timePeriod** | array | A set of time periods. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1) |
| id |string | A unique identifier for a temporal element. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-0) |
| description |string | Text associated with the time instance. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-1) |
| beginPosition |string | Starting date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-2) |
| endPosition |string | Ending date, or date and time. | false | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-3-1-0-3) |

##userContactInfo
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **userContactInfo** | array | Identification of and means of communicating with the person(s) and organization(s) using the resource. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-0-1) |

##version
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **version** | object | Identifies the version of the JSON schema standard that applies to the metadata. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0) |
| name |string | Schema identifier, i.e. the name of the schema standard. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-0) |
| version |string | Specific version number of the schema standard. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-1) |

##verticalElement
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **verticalElement** | array | Vertical element of an extent. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2) |
| minimumValue |number | Lowest vertical extent contained in the dataset. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-0) |
| maximumValue |number | Highest vertical extent contained in the dataset. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-1) |
| verticalCRSTitle |string | Name of a geographic reference system associated with a vertical extent. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-2) |
| verticalCRSUri |string | Web link to the parameters for a geographic reference system associated with a vertical extent. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2-0-3) |

##voucher
| Name | Type | Description | Required | Viewer Link|
|---|---|---|---|---|
| **voucher** | object | Information on the types of specimen, the repository, and the individuals who identified the vouchers. |   | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4) |
| specimen |string | Word or phrase describing the type of specimen collected (e.g. herbarium specimens, blood samples, photographs, individuals, or batches). Example: "herbarium specimens", "blood samples", "photographs", "individuals", "free text". | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-0) |
| repository |object | Information about the curator or contact person and/or agency responsible for the specimens. | true | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-4-1) |
