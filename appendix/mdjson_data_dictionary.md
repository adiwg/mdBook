# mdJSON Data Dictionary

<!-- toc -->

##additionalDocumentation
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **additionalDocumentation** | array | Other documents related to, but not defining, the resource such as factsheets, data catalog pages, award documents, proposals, and informational websites. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |
| resourceType |string | Identifies the type of resource, such as: userGuide, website, report, etc. | false | <ul><li>ISO 19115-2<ul><li>[MD_ScopeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0) |
| citation |object | schema for citation | false | <ul><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1) |

##address
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **address** | object | Physical and email address at which the organization or individual may be contacted. |   | <ul><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; contactInfo &gt; CI_Contact &gt; address &gt; CI_Address</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2) |
| deliveryPoint |array | Address line for the location. | false | <ul><li>ISO 19115-2<ul><li>CI_Address &gt; deliveryPoint</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; address</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-0) |
| city |string | City of the location. | false | <ul><li>ISO 19115-2<ul><li>CI_Address &gt; city</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; city</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-1) |
| administrativeArea |string | State, province of the location. | false | <ul><li>ISO 19115-2<ul><li>CI_Address &gt; administrativeArea</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; state</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-2) |
| postalCode |string | ZIP or other postal code. | false | <ul><li>ISO 19115-2<ul><li>CI_Address &gt; postalCode</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; postal</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-3) |
| country |string | ZIP or other postal code. | false | <ul><li>ISO 19115-2<ul><li>CI_Address &gt; postalCode</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; postal</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-4) |
| electronicMailAddress |array | E-mail or electronic mailbox address. | false | <ul><li>ISO 19115-2<ul><li>CI_Address &gt; electronicMailAddress</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntemail</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2-5) |

##associatedResource
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **associatedResource** | array | Other resources which are directly related to the subject resource such as parent, child, or sibling datasets or projects. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| associationType |string | Identifies how the associated resource is related to the subject resource such as 'is a component of', 'larger work citation', 'cross reference', etc. | true | <ul><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; associationType [DS_AssociationTypeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-0) |
| initiativeType |string | Identifies type of initiative under which the resource was produced - the activity that resulted in the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; initiativeType &gt; [DS_InitiativeTypeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1) |
| resourceType |string | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | <ul><li>ISO 19115-2<ul><li>[MD_ScopeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-2) |
| resourceCitation |object | Citation for the associated resource. | false | <ul><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref &gt; citeinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3) |
| metadataCitation |object | Citation for the associated resource metadata. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4) |

##attribute
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **attribute** | array | An array of objects defining the attributes for the entity |   | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7) |
| commonName |string | The common name used to identify this attribute | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; memberName &gt; localName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-0) |
| codeName |string | The code used to identify this attribute.  Most often this will be the table or spreadsheet column name | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; code &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-1) |
| alias |array | An array of quoted strings providing alternate names by which the attribute is known | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-2) |
| definition |string | A succinct but comprehensive definition for the attribute | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; definition &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-3) |
| dataType |string | The datatype for the attribute.  Names for datatypes vary widely by database management system.  Use the datatype name associated with the database system that implemented the entity.  E.g. 'integer', 'boolean', 'decimal(8,5)', 'varchar(200)' | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; valueType &gt; TypeName &gt; aName &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-4) |
| allowNull |boolean | Indicates whether null values are allowed for the attribute | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; cardinality &gt; Multiplicity &gt; range &gt; MultiplicityRange &gt; lower &gt; integer[0=optional &#124; 1=required]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-5) |
| units |string | A unit-of-measure for the attribute.  E.g. 'meters', 'atmospheres', 'liters' | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; valueMeasurementUnit &gt; [UnitDefinition &gt; identifier &#124; ConversionalUnit &gt; identifier, name, catalogSystem, conversionToPreferredUnit, formula | BaseUnit &gt; identifier, name, catalogSymbol, unitSystem | DerivedUnit &gt; identifier, name, remarks, catalogSymbol, derivationUnitTerm]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-6) |
| domainId |string | Provides the domain ID for the  dictionary Domain containing the list of permissable values for this attribute | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-7) |
| minValue |string | The minimum range value permissible for this attribute | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-8) |
| maxValue |string | The maximum range value permissible for this attribute | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7-0-9) |

##authority
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **authority** | object | Citation for the authority issuing the identifier. |   | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-5) |
| title |string | Name by which the cited resource is known. | true | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-5-0) |
| alternateTitle |string | Alias by which the cited resource is known. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-5-1) |
| date |array | Date referenced to the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-5-2) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-5-3) |
| onlineResource |array | On-line information related to the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-5-4) |

##citation
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **citation** | object | Citation for the dictionary. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0) |
| edition |string | Version identifier for the dictionary. | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-0) |
| title |string | Name by which the cited resource is known. | true | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-0) |
| alternateTitle |string | Alias by which the cited resource is known. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-1) |
| date |array | Date referenced to the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3) |
| onlineResource |array | On-line information related to the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-4) |

##classificationSystem
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **classificationSystem** | array | Information (citation) about the taxonomic classification system or authority used. |   | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; classSys &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; classsys</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0) |
| edition |string | Version identifier for the resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-2) |
| title |string | Name by which the cited resource is known. | true | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-3-0-0) |
| alternateTitle |string | Alias by which the cited resource is known. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-3-0-1) |
| date |array | Date referenced to the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-3-0-2) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-3-0-3) |
| onlineResource |array | On-line information related to the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0-0-0-0-3-0-4) |

##classifiedDataItem
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **classifiedDataItem** | array | Information about thematic classification item(s). |   | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription &gt; gmi:rangeElement</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11-1) |
| className |string | The name of the thematic classification item. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription &gt; gmi:rangeElement  &gt; gco:Record &gt; gmd:RS_Identifier &gt; gmd:authority &gt; gmd:CI_Citation &gt; gmd:title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11-1-0-0) |
| classDescription |string | The description of the thematic classification item. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription &gt; gmi:rangeElement  &gt; gco:Record &gt; gmd:RS_Identifier &gt; gmd:authority &gt; gmd:CI_Citation &gt; gmd:alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11-1-0-1) |
| classValue |number | The thematic classification value. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription &gt; gmi:rangeElement  &gt; gco:Record &gt; gmd:RS_Identifier &gt; gmd:code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11-1-0-2) |

##classifiedData
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **classifiedData** | object | The information about the thematic classification used with this coverage item. |   | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11) |
| numberOfClasses |integer | The number of values used in a thematic classification resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11-0) |
| classifiedDataItem |array | Information about thematic classification item(s). | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription &gt; gmi:rangeElement</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11-1) |

##constraint
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **constraint** | object | Provides information about constraints to the use of the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| useLimitation |array | Limitation affecting the fitness for use of the resource or metadata. For example, "not to be used for navigation". | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceConstraints &gt; MD_Constraints[useLimitation]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0) |
| legalConstraint |array | Restrictions and legal prerequisites for accessing and using the resource or metadata. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; resourceConstraints &gt; MD_LegalConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1) |
| securityConstraint |array | Handling restrictions imposed on the resource or metadata for national security or similar security concerns. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; resourceConstraints &gt; MD_SecurityConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2) |

##contact
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **contact** | array | An array of contacts to be referenced throughout the metadata. Any contact used in the metadata record must be stored within this array and referenced by contactId. Items in array may be used 0-n times throughout the record. |   | <ul><li>ISO 19115-2<ul><li>Contact &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>[single member of array] = cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1) |
| individualName |string | Name of the person - surname, given name, title separated by a delimiter. | true | <ul><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; individualName</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntperp &gt; cntper</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-0-0) |
| contactId |string | Unique identifier for the contact. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-0) |
| positionName |string | Role or position of the person, usually within a given organization. | false | <ul><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; positionName</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-1) |
| address |object | Physical and email address at which the organization or individual may be contacted. | false | <ul><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; contactInfo &gt; CI_Contact &gt; address &gt; CI_Address</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-2) |
| onlineResource |array | Information about accessing on-line resources and services. This may be a website, profile page, GitHub page, etc. related to the contact. | false | <ul><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; contactInfo &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-3) |
| contactInstructions |string | Supplemental instructions on how or when to contact the individual or organization. | false | <ul><li>ISO 19115-2<ul><li>CI_Contact &gt; contactInstructions</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntinst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-4) |
| phoneBook |array | Supplemental instructions on how or when to contact the individual or organization. | false | <ul><li>ISO 19115-2<ul><li>CI_Contact &gt; contactInstructions</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntinst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5) |
| organizationName |string | Name of the organization. | true | <ul><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; organisationName</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntperp &gt; cntorg</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-0) |

##coverageInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **coverageInfo** | array | Details about the content of a raster(grid) resource. |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; contentInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28) |
| coverageType |string | Type of information represented by the cell values | true | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &#124; MI_CoverageDescription &gt; contentType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-0) |
| coverageName |string | The name(title) of the coverage. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &#124; MI_CoverageDescription &gt; attributeDescription &gt; gco:RecordType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-1) |
| coverageDescription |string | A description of the coverage | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &#124; MI_CoverageDescription &gt; attributeDescription &gt; gco:RecordType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-2) |
| processingLevel |object | Code that identifies the level of radiometric and geometric processing that has been applied. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; processingLevelCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3) |
| coverageItem |array | Information about the item(s) described by the grid cell. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; [gmi:rangeElementDescription &#124; gmd:dimension]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4) |
| imageInfo |object | Information about the image. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5) |

##coverageItem
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **coverageItem** | array | Information about the item(s) described by the grid cell. |   | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; [gmi:rangeElementDescription &#124; gmd:dimension]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4) |
| itemName |string | Coverage item name. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription &gt; gmi:name</li><li>MI_CoverageDescription &gt;  gmd:dimension &gt; gmd:MD:Band &gt; gmd:sequenceIdentifier &gt; gco:MemberName &gt; gco:aName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-0) |
| itemType |string | The type of value for the coverage item. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD:Band &gt; gmd:sequenceIdentifier &gt; gco:MemberName &gt; gco:attributeType &gt; gco:TypeName &gt; gco:aName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-1) |
| itemDescription |string | Description of the coverage item. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription &gt; gmi:definition</li><li>MI_CoverageDescription &gt;  gmd:dimension &gt; gmd:MD_Band &gt; gmd:descriptor ]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-2) |
| minValue |number | The minimum value of data values in the domain of the coverage item. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:minValue &gt; gco:Real</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-3) |
| maxValue |number | The maximum value of data values in the domain of the coverage item | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:maxValue &gt; gco:Real</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-4) |
| units |string | The units of data in which the coverage item is expressed. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:units &gt; gml:unitDefinition &gt; gml:identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-5) |
| scaleFactor |number | The scale factor which has been applied to the coverage item | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:scaleFactor &gt; gco:Real</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-6) |
| offset |number | The physical value corresponding to a coverage item value of zero. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:offset &gt; gco:Real</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-7) |
| meanValue |number | The mean value of data values in the coverage item. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-8) |
| standardDeviation |number | The standard deviation of data values in the coverage item. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-9) |
| bitsPerValue |integer | The maximum number of significant bits in the uncompressed representation for the value in each pixel. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:bitsPerValue &gt; gco:Integer</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-10) |
| classifiedData |object | The information about the thematic classification used with this coverage item. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt;  gmi:rangeElementDescription &gt; gmi:MI_RangeElementDescription</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-11) |
| sensorInfo |object | Information about the sensor that collected the grid cell values. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmi:rangeElementDescription &#124; gmd:dimension</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-12) |

##dataDictionary
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **dataDictionary** | array | A description of the contents, format and structure of the physical objects in a data resource. |   | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3) |
| dictionaryInfo |object | Identification, description, and contact information for the data dictionary. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0) |
| domain |array | A list of permissable values used to constrain an attribute's value.  A single domain may be assigned to multiple attributes in a table or database. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1) |
| entity |array | Defines the structure of a discrete data object within the data resource.  The data object may be a table, dataset, or single sheet of a spreadsheet. | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2) |

##dataQualityInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **dataQualityInfo** | array | Information that describes the data quality, lineage, and/or processing steps that were applied to the whole or part of the data resource. |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; dataQualityInfo &gt; DQ_DataQuality</li></ul></li><li>FGDC CSDGM<ul><li>dataqual</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29) |
| scope |string | The scope to which the data quality information is applied, for instance; dataset, attribute, feature, series, etc. | true | <ul><li>ISO 19115-2<ul><li>DQ_DataQuality &gt; scope &gt; DQ_Scope &gt; level &gt; MD_ScopeCode</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-0) |
| lineage |object | Procedural (non-quantitative) data quality information about the portion of the data resource identified by the data quality scope. | false | <ul><li>ISO 19115-2<ul><li>DQ_DataQuality &gt; lineage &gt; LI_Lineage</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1) |

##date
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **date** | array | Date referenced to the cited resource. |   | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2) |
| date |string | An ISO 8601 date/timestamp. | true | <ul><li>ISO 19115-2<ul><li>CI_Date &gt; date</li><li>FC_FeatureCatalogue &gt; versionDate</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; pubdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2-0-0) |
| dateType |string | The type of date in the context of the citation. | true | <ul><li>ISO 19115-2<ul><li>CI_Date &gt; dateType [CI_DateTypeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-2-0-1) |

##dictionaryInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **dictionaryInfo** | object | Identification, description, and contact information for the data dictionary. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0) |
| citation |object | Citation for the dictionary. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0) |
| resourceType |string | Identifies the scope of the data dictionary. E.g. 'database', 'dataset', 'table'. | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; scope</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-1) |
| description |string | A brief description of the data dictionary and its source. | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; fieldOfApplication &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-2) |
| language |string | Defines the language and country of origin in which the data dictionary is written.  E.g. 'eng; USA', 'eng; UK', 'esp; MEX'. | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-3) |
| includedWithDataset |boolean | Indication of whether or not the data dictionary is included with the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_FeatureCatalogueDescription &gt; includedWithDataset</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-4) |

##dimension
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **dimension** | array | Information about spatial-temporal axis properties. |   | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1) |
| dimensionType |string | The type of dimension for this axis. | true | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; dimensionName &gt; MD_DimensionNameTypeCode</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1-0-0) |
| dimensionSize |integer | The number of elements along the axis. | true | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; dimensionSize</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1-0-1) |
| resolution |number | Numeric Value that defines the degree of detail in the grid. | false | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; resolution</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1-0-2) |
| resolutionUnit |string | Unit of measure for the resolution. | false | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; resolution @uom</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1-0-3) |
| dimensionTitle |string | The name of the axis. | false | <ul><li>ISO 19115-2<ul><li></li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1-0-4) |
| dimensionDescription |string | The description of the axis. | false | <ul><li>ISO 19115-2<ul><li></li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1-0-5) |

##distributionInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **distributionInfo** | array | Information about the distributor of and options for obtaining the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_Metadata &gt; distribution &gt; MD_Distribution</li></ul></li><li>FGDC CSDGM<ul><li>distinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| distributorContact |object | Party from whom the resource may be obtained. Note: This list need not be exhaustive. | true | <ul><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorContact &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; distrib &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0) |
| distributionOrderProcess |array | Provides information about how the resource may be obtained and related instructions and fee information. | false | <ul><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributionOrderProcess &gt; MD_StandardOrderProcess</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1) |
| distributorFormat |array | Provides information about the format used by the distributor. Deprecated: moved to distributorTransferOptions. | false | <ul><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorFormat &gt; MD_Format</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2) |
| distributorTransferOptions |array | Describes method and media by which a resource is obtained from the distributor. | false | <ul><li>ISO 19115-2<ul><li>MD_Distributor &gt; distributorTransferOptions &gt; MD_DigitalTransferOptions</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |

##distributionOrderProcess
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **distributionOrderProcess** | array | Provides information about how the resource may be obtained and related instructions and fee information. |   | <ul><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributionOrderProcess &gt; MD_StandardOrderProcess</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1) |
| fees |string | Fees and terms for retrieving the resource, including monetary units. | false | <ul><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; fees</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; fees</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-0) |
| plannedAvailabilityDateTime |string | Date and time when the resource will be available. | false | <ul><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; plannedAvailabilityDateTime</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-1) |
| orderingInstructions |string | General instructions, terms and services provided by the distributor. | false | <ul><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; orderingInstructions</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; onlinopt &gt; accinstr</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-2) |
| turnaround |string | Typical turnaround time for the filling of an order. | false | <ul><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; turnaround</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; turnarnd</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1-0-3) |

##distributorContact
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **distributorContact** | object | Party from whom the resource may be obtained. Note: This list need not be exhaustive. |   | <ul><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorContact &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; distrib &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0-1) |

##distributorFormat
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **distributorFormat** | array | Provides information about the format used by the distributor. |   | <ul><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorFormat &gt; MD_Format</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0) |
| compressionMethod |string | Method used to compress the format. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-0) |
| formatName |string | Name of the data transfer format. | true | <ul><li>ISO 19115-2<ul><li>MD_Format &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtinfo &gt; formname</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-1-0-0) |
| version |string | Version of the format (date, number, etc.) | false | <ul><li>ISO 19115-2<ul><li>MD_Format &gt; version</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0-0-1-0-1) |

##distributorTransferOptions
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **distributorTransferOptions** | array | Describes method and media by which a resource is obtained from the distributor. |   | <ul><li>ISO 19115-2<ul><li>MD_Distributor &gt; distributorTransferOptions &gt; MD_DigitalTransferOptions</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |
| distributorFormat |array | Provides information about the format used by the distributor. | false | <ul><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorFormat &gt; MD_Format</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0) |
| transferSize |number | Total size of the transfer. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1) |
| transferSizeUnits |enum: kB, KB, MB, GB, TB | Units of transfer size. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-2) |
| online |array | Information about obtaining the resource on-line. | false | <ul><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; online &gt; CI_OnlineResource</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; onlinopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3) |
| offline |object | Information about obtaining the resource through off-line procedure. | false | <ul><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; offline &gt; MD_Medium</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4) |

##domain
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **domain** | array | A list of permissable values used to constrain an attribute's value.  A single domain may be assigned to multiple attributes in a table or database. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1) |
| domainId |string | A user provided unique ID for this domain.  The ID will be used to locate the domain in the domain array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-0) |
| commonName |string | A short common name for the domain. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-1) |
| codeName |string | The code or 'lookup table' name for the domin used in the database schema definitions. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-2) |
| description |string | A brief description of the domain including identification of any established sources used in creating the list of domain items. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-3) |
| member |array | An array of member objects that enumerate and define the valid values for a domain. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4) |

##entity
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **entity** | array | Defines the structure of a discrete data object within the data resource.  The data object may be a table, dataset, or single sheet of a spreadsheet. |   | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2) |
| entityId |string | A user provided unique ID for this entity.   | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType#id=''</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-0) |
| commonName |string | The name commonly used to identify this entity | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; typeName &gt; localName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-1) |
| codeName |string | The code name used to identify this entity in a database schema or application software. For spreasheets this would likely be the sheet name.  | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; code &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-2) |
| alias |array | An array of quoted strings providing alternate names used to identify this entity | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; aliases &gt; localName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-3) |
| definition |string | A brief definition for the entity | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; definition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-4) |
| primaryKeyAttributeCodeName |array | An array of quoted attribute code names that together compose the primary key set for the entity | false | <ul><li>ISO 19115-2<ul><li>Note: the primary key is written as a text description into FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-5) |
| index |array | An array of objects describing alternate indexes for the entity | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; Note: the index is written as a text description into featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6) |
| attribute |array | An array of objects defining the attributes for the entity | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-7) |
| foreignKey |array | An array of objects describing attributes whose values are restricted to values found in the domain of an attribute belonging to another table or dataset | false | <ul><li>ISO 19115-2<ul><li>Note: the foreign key is written as a text description into FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8) |

##epsgNumber
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **epsgNumber** | array | The EPSG Geodetic Parameter Dataset of the reference system, see epsg-registry.org. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-1) |

##extent
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **extent** | array | Information about the geographic, vertical, and temporal extent of the resource. A resource may have multiple extents. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; extent &gt; EX_Extent</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26) |
| description |string | Description of the geographic extent. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-0) |
| geographicElement |array | An array of objects each describing a geographic boundary or location comprising all or a portion of the resource. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1) |
| verticalElement |array | An array of objects each describing a vertical boundary comprising all or a portion of the resource. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; verticalElement &gt; EX_VerticalExtent </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-2) |
| temporalElement |object | An array of objects each describing a temporal boundary comprising all or a portion of the resource. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; temporalElement &gt; EX_TemporalExtent</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3) |

##features
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **features** | array | Set of Features constituting the FeatureCollection. |   | <ul><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; MultiGeometry</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3) |
| type |enum: Feature | Type of GeoJSON object. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-0) |
| geometry |ambiguous | The geometry object associated with the Feature. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-1) |
| properties |ambiguous | JSON object containing information about a feature or collection. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2) |
| id |string,number | Unique identifier for the GeoJSON feature object. | false | <ul><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; [Point, LineString, Polygon] @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-3) |

##foreignKey
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **foreignKey** | array | An array of objects describing attributes whose values are restricted to values found in the domain of an attribute belonging to another table or dataset |   | <ul><li>ISO 19115-2<ul><li>Note: the foreign key is written as a text description into FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8) |
| localAttributeCodeName |array | An array of local (referencing or child) attribute code names for this foreign key | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-0) |
| referencedEntityCodeName |string | The entityID for the referenced (or parent) entity for this foreign key | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-1) |
| referencedAttributeCodeName |array | An array of referenced (or parent) attribute code names for this foreign key.  If the foreign key is compound key (more than one attribute compose the key) the order of the referenced attributes must allign precicely with the order and number of local attributes. | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-8-0-2) |

##geographicElement
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **geographicElement** | array | An array of objects each describing a geographic boundary or location comprising all or a portion of the resource. |   | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1) |
| type |enum: FeatureCollection | Type of GeoJSON object. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-0) |
| crs |ambiguous | The coordinate reference system (CRS) of a GeoJSON object. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-0) |
| bbox |array | To include information on the coordinate range for geometries, features, or feature collections, a GeoJSON object may have a member named "bbox". The value of the bbox member must be a 2*n array where n is the number of dimensions represented in the contained geometries, with the lowest values for all axes followed by the highest values. The axes order of a bbox follows the axes order of geometries. In addition, the coordinate reference system for the bbox is assumed to match the coordinate reference system of the GeoJSON object of which it is a member. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement &gt; EX_GeographicBoundingBox, EX_GeographicBoundingBox &gt; westBoundLongitude &gt; Decimal {west}, EX_GeographicBoundingBox &gt; eastBoundLongitude &gt; Decimal {east}, EX_GeographicBoundingBox &gt; southBoundLatitude &gt; Decimal {south}, EX_GeographicBoundingBox &gt; northBoundLatitude &gt; Decimal {north}</li></ul></li><li>FGDC CSDGM<ul><li>[idinfo &gt; spdom &gt; bounding &gt; westbc], [idinfo &gt; spdom &gt; bounding &gt; eastbc], [idinfo &gt; spdom &gt; bounding &gt; northbc], [idinfo &gt; spdom &gt; bounding &gt; southbc]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-1) |
| coordinates |array | The set of Polygons that constitute the MultiPolygon. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; MultiGeometry &gt; geometryMembers &gt; Polygon[ ] &gt; [exterior &gt; LinearRing &gt; coordinates &#124; interior[ ] &gt; LinearRing &gt; coordinates]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-0-0-5-1) |
| geometries |array | The set of geometry objects constituting the GeometryCollection. | true | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; MultiGeometry &gt; geometryMembers</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-1-1) |
| geometry |ambiguous | The geometry object associated with the Feature. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-2-1) |
| properties |ambiguous | JSON object containing information about a feature or collection. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-1) |
| id |string,number | Unique identifier for the GeoJSON object. | false | <ul><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; [Point, LineString, Polygon] @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-2) |
| features |array | Set of Features constituting the FeatureCollection. | true | <ul><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; MultiGeometry</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3) |

##graphicOverview
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **graphicOverview** | array | Provides a path or link to images, maps, flow charts, models, etc. that illustrate the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; graphicOverview &gt; MD_BrowseGraphic</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20) |
| fileName |string | Name of the file that contains a graphic overview of the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsen</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-0) |
| fileDescription |string | Description of the graphic overview. | false | <ul><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileDescription</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsed</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-1) |
| fileType |string | The format in which the illustration is encoded such as GIF, JPEG, PBM, PS, TIFF. | false | <ul><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileType</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browset</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2) |
| fileUri |string | URI of the graphic overview. | false | <ul><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename @xlink:href</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-3) |

##gridInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **gridInfo** | array | Information about grid objects in the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27) |
| numberOfDimensions |number | The number of independent spatial-temporal axes. | true | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; numberOfDimensions</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-0) |
| dimension |array | Information about spatial-temporal axis properties. | true | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-1) |
| cellGeometry |string | Identification of grid data as point or cell. | true | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; cellGeometry</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-2) |
| transformationParameterAvailability |boolean | An indication of whether or not parameters for transformation between image coordinates and geographic or map coordinates exist (are available). | false | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; transformationParameterAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27-0-3) |

##identifier
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **identifier** | array | Identifier for the resource in the context of the citation. |   | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2) |
| identifier |string | A name that is used to identify the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-1) |
| version |string | The version of the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-3) |
| type |string | The type of identifier, e.g. doi, isbn, issn, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; ISBN</li><li>CI_Citation &gt; ISSN</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-4) |
| authority |object | Citation for the authority issuing the identifier. | false | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-1-0-0-2-0-5) |

##imageInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **imageInfo** | object | Information about the image. |   | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5) |
| illuminationElevationAngle |number | Illumination elevation measured in degrees clockwise from the target plane at intersection of the optical line of sight with the Earth’s surface. For images from a scanning device, refer to the centre pixel of the image. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; illiminationElevationAngle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-0) |
| illuminationAzimuthAngle |number | Illumination azimuth measured in degrees clockwise from true north at the time the image is taken. For images from a scanning device, refer to the centre pixel of the image | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; illuminationAzimuthAngle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-1) |
| imagingCondition |string | Code which indicates conditions which may affect the image. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; imageCondition &gt; MD_ImageConditionCode</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-2) |
| imageQuality |object | Specifies the image quality. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; imageQualityCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3) |
| cloudCoverPercent |number | Area of the dataset obscured by clouds, expressed as a percentage of the spatial extent. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; cloudCoverPercentage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-4) |
| compressionQuantity |number | Count of the number of lossy compression cycles performed on the image. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; compressionGenerationQuality</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-5) |
| triangulationIndicator |boolean | Indication of whether or not triangulation has been performed upon the image. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; triangulationIndicator</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-6) |
| radiometricCalibrationAvailable |boolean | Indication of whether or not the radiometric calibration information for generating the radiometrically calibrated standard data product is available. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; radiometricCalibrationDataAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-7) |
| cameraCalibrationAvailable |boolean | Indication of whether or not constants are available which allow for camera calibration corrections. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; camerCalibrationInformationAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-8) |
| filmDistortionAvailable |boolean | Indication of whether or not Calibration Reseau information is available | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; filmDistrotionInformationAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-9) |
| lensDistortionAvailable |boolean | Indication of whether or not lens aberration correction information is available. | false | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; lensDistortionInformationAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-10) |

##imageQuality
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **imageQuality** | object | Specifies the image quality. |   | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; imageQualityCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3) |
| identifier |string | A name that is used to identify the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3-1) |
| version |string | The version of the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3-3) |
| type |string | The type of identifier, e.g. doi, isbn, issn, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; ISBN</li><li>CI_Citation &gt; ISSN</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3-4) |
| authority |object | Citation for the authority issuing the identifier. | false | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-5-3-5) |

##index
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **index** | array | An array of objects describing alternate indexes for the entity |   | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; Note: the index is written as a text description into featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6) |
| codeName |string | The code name used to define the alternate index on the entity | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-0) |
| allowDuplicates |boolean | Indicates whether the index allows duplicates or values are required to be unique.  true = allow duplicates; false = values must be unique. | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-1) |
| attributeCodeName |array | An array of quoted attribute code names that together compose an alternate key set for the entity | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2-0-6-0-2) |

##keyword
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **keyword** | array | Provides category keywords, their type, and reference source. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; descriptiveKeywords &gt; MD_Keywords</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; keywords</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| keyword |array | Commonly used word(s) or formalized word(s) or phrase(s) used to describe the subject. | true | <ul><li>ISO 19115-2<ul><li>MD_Keywords &gt; keyword</li></ul></li><li>FGDC CSDGM<ul><li>idinfo&gt;keywords&gt;theme&gt;themekey</li><li>idinfo&gt;keywords&gt;place&gt;placekey</li><li>idinfo&gt;keywords&gt;temporal&gt;tempkey</li><li>idinfo&gt;keywords&gt;stratum&gt;stratkey</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-0) |
| keywordType |string | A code, or concept, that defines the subject matter used to group similar keywords. | false | <ul><li>ISO 19115-2<ul><li>MD_Keywords &gt; type</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-1) |
| thesaurus |object | Name of the formally registered thesaurus or a similar authoritative source of keywords. | false | <ul><li>ISO 19115-2<ul><li>MD_Keywords &gt; thesaurusName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo&gt;keywords&gt;theme&gt;themekt</li><li>idinfo&gt;keywords&gt;place&gt;placekt</li><li>idinfo&gt;keywords&gt;temporal&gt;tempkt</li><li>idinfo&gt;keywords&gt;stratum&gt;stratkt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2) |

##legalConstraint
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **legalConstraint** | array | Restrictions and legal prerequisites for accessing and using the resource or metadata. |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; resourceConstraints &gt; MD_LegalConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1) |
| accessConstraint |array | Access constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations on obtaining the resource or metadata. | false | <ul><li>ISO 19115-2<ul><li>MD_LegalConstraints &gt; accessConstraints [MD_RestrictionCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; accconst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1-0-0) |
| useConstraint |array | Constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations or warnings on using the resource or metadata. | false | <ul><li>ISO 19115-2<ul><li>MD_LegalConstraints &gt; useConstraints [MD_RestrictionCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; useconst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1-0-1) |
| otherConstraint |array | Other restrictions and legal prerequisites for accessing and using the resource or metadata. | false | <ul><li>ISO 19115-2<ul><li>MD_LegalConstraints &gt; otherConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-1-0-2) |

##lineage
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **lineage** | object | Procedural (non-quantitative) data quality information about the portion of the data resource identified by the data quality scope. |   | <ul><li>ISO 19115-2<ul><li>DQ_DataQuality &gt; lineage &gt; LI_Lineage</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1) |
| statement |string | A general statement of the actions taken to verify, transform, repair, and integrate the data within the data quality scope. | false | <ul><li>ISO 19115-2<ul><li>LI_Lineage &gt; statement</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-0) |
| processStep |array | A brief statement describing an individual, non-trivial process or methodology step taken in development of the resource data within the data quality scope. | false | <ul><li>ISO 19115-2<ul><li>LI_Lineage &gt; processStep &gt; LI_ProcessStep</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-1) |
| source |array | Information about the source data used in creating the data identified by the data quality scope. | false | <ul><li>ISO 19115-2<ul><li>LI_Lineage &gt; source &gt; LI_Source</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; srcinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2) |

##locale
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **locale** | array | Localised language(s) and characterset(s) used within the resource. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11) |
| language |string | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11-0-0) |
| characterSet |string | Full name of the character encoding standard used by the resource(see http://www.iana.org/assignments/character-sets/character-sets.xhtml). | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11-0-1) |
| country |string | Designation of the specific country of the locale language(ISO 3166-1). | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11-0-2) |

##maintenanceContact
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **maintenanceContact** | array | Contact information for the maintainer of the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; contact &gt; CI_Contact</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-2-0-1) |

##member
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **member** | array | An array of member objects that enumerate and define the valid values for a domain. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4) |
| name |string | A descriptive name associated with a domain value | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; listedValue &gt; FC_ListedValue &gt; label</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-0) |
| value |string | A descriptive name associated with a domain value | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; listedValue &gt; FC_ListedValue &gt; label</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-1) |
| definition |string | A brief definition for the domain item | true | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; listedValue &gt; FC_ListedValue &gt; definition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1-0-4-0-2) |

##metadataCitation
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **metadataCitation** | object | Citation for the associated resource metadata. |   | <ul><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4) |
| edition |string | Version identifier for the resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-2) |
| title |string | Name by which the cited resource is known. | true | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-0) |
| alternateTitle |string | Alias by which the cited resource is known. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-1) |
| date |array | Date referenced to the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-2) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-3) |
| onlineResource |array | On-line information related to the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-4-0-0-3-0-4) |

##metadataContact
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **metadataContact** | array | Person or organization responsible for metadata information (metadata custodian). |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; contact &gt; CI_Contact &gt; responsibleParty &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-0-1) |

##metadataIdentifier
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **metadataIdentifier** | object | Unique identifier for this metadata file. |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; fileIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| identifier |string | A name that is used to identify the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-1) |
| version |string | The version of the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-3) |
| type |string | The type of identifier, e.g. doi, isbn, issn, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; ISBN</li><li>CI_Citation &gt; ISSN</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-4) |
| authority |object | Citation for the authority issuing the identifier. | false | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-5) |

##metadataInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **metadataInfo** | object | General information about the metadata record. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| metadataIdentifier |object | Unique identifier for this metadata file. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; fileIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| parentMetadata |object | Identifier of the metadata to which this metadata is a subset (child). | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; parentIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| metadataContact |array | Person or organization responsible for metadata information (metadata custodian). | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; contact &gt; CI_Contact &gt; responsibleParty &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| metadataCharacterSet |string | Full name of the character coding standard used for the metadata set. NOTE:This property has been deprecated in favor of 'metadataLocale'. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3) |
| metadataLocale |array | Localised language(s) and characterset(s) used within the metadata record. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4) |
| metadataCreationDate |string | Date that the metadata was created. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; dateStamp</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metd</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5) |
| metadataLastUpdate |string | Date that the metadata was updated. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; dateStamp</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metrd</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6) |
| metadataUri |string | Uniform Resource Identifier (URI) of the metadata record. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; linkage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7) |
| metadataStatus |string | Status of the metadata record. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8) |
| metadataMaintenance |object | Provides information about the frequency of metadata updates, and the scope of those updates. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; metadataMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9) |

##metadataLocale
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **metadataLocale** | array | Localised language(s) and characterset(s) used within the metadata record. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4) |
| language |string | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4-0-0) |
| characterSet |string | Full name of the character encoding standard used by the resource(see http://www.iana.org/assignments/character-sets/character-sets.xhtml). | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4-0-1) |
| country |string | Designation of the specific country of the locale language(ISO 3166-1). | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4-0-2) |

##metadataMaintenance
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **metadataMaintenance** | object | Provides information about the frequency of metadata updates, and the scope of those updates. |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; metadataMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9) |
| maintenanceFrequency |string | Describes the frequency of additions and updates made to a resource. | false | <ul><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceAndUpdateFrequency [MD_MaintenanceFrequencyCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-0) |
| maintenanceNote |array | Notes regarding the maintenance of the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceNote</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-1) |
| maintenanceContact |array | Contact information for the maintainer of the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; contact &gt; CI_Contact</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-2) |

##metadata
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **metadata** | object | The main body of the metadata record. |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata</li></ul></li><li>FGDC CSDGM<ul><li>metadata</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2) |
| metadataInfo |object | General information about the metadata record. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| resourceInfo |object | Information about the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_Metadata &gt; identificationInfo &gt; MD_DataIdentification</li></ul></li><li>FGDC CSDGM<ul><li>idinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| distributionInfo |array | Information about the distributor of and options for obtaining the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_Metadata &gt; distribution &gt; MD_Distribution</li></ul></li><li>FGDC CSDGM<ul><li>distinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| associatedResource |array | Other resources which are directly related to the subject resource such as parent, child, or sibling datasets or projects. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| additionalDocumentation |array | Other documents related to, but not defining, the resource such as factsheets, data catalog pages, award documents, proposals, and informational websites. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |

##observer
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **observer** | array | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. |   | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; obs &gt; CI_ResponsibleParty</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-2-0-1) |

##offline
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **offline** | object | Information about obtaining the resource through off-line procedure. |   | <ul><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; offline &gt; MD_Medium</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4) |
| name |string | Name of the format the data is distributed in, such as: dvd, hardcopy, etc. | false | <ul><li>ISO 19115-2<ul><li>MD_Medium &gt; name [MD_MediumNameCode]</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn &gt; offmedia</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4-0) |
| mediumCapacity |number | Total capacity of the storage format. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4-1) |
| mediumCapacityUnits |enum: kB, KB, MB, GB, TB | Units of medium capacity. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4-2) |
| mediumFormat |string | Method used by the resource provider to write to the medium, such as: tar, iso9660, etc. | false | <ul><li>ISO 19115-2<ul><li>MD_Medium &gt; mediumFormat [MD_MediumFormatCode]</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn &gt; recfmt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4-3) |
| mediumNote |string | Description of other limitations or requirements for using the medium. | false | <ul><li>ISO 19115-2<ul><li>MD_Medium &gt; mediumNote</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn &gt; compat</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4-4) |

##onlineResource
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **onlineResource** | array | On-line information related to the citation. |   | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-4) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; linkage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-4-0-0) |
| name |string | Name of the online resource. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; name</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-4-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; protocol</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-4-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-4-0-3) |
| function |string | Function performed by the online resource. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; function &gt; CI_OnlineFunctionCode [codelist]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-4-0-4) |

##online
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **online** | array | Information about obtaining the resource on-line. |   | <ul><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; online &gt; CI_OnlineResource</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; onlinopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; linkage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3-0-0) |
| name |string | Name of the online resource. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; name</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; protocol</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3-0-3) |
| function |string | Function performed by the online resource. | false | <ul><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; function &gt; CI_OnlineFunctionCode [codelist]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3-0-4) |

##parentMetadata
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **parentMetadata** | object | Identifier of the metadata to which this metadata is a subset (child). |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; parentIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| edition |string | Version identifier for the resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-2) |
| title |string | Name by which the cited resource is known. | true | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-0) |
| alternateTitle |string | Alias by which the cited resource is known. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-1) |
| date |array | Date referenced to the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-2) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-3) |
| onlineResource |array | On-line information related to the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3-0-4) |

##phoneBook
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **phoneBook** | array | Supplemental instructions on how or when to contact the individual or organization. |   | <ul><li>ISO 19115-2<ul><li>CI_Contact &gt; contactInstructions</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntinst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5) |
| phoneName |string | Descriptive name of the phone number. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-0) |
| phoneNumber |string | Telephone number. Recommended format is to use 'x' or 'ext' to denote extensions. | true | <ul><li>ISO 19115-2<ul><li>CI_Telephone &gt; voice &#124; facsimile</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntvoice</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-1) |
| service |array | Type(s) of phone number, e.g. voice, sms. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-1-1-0-5-0-2) |

##pointOfContact
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **pointOfContact** | array | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; pointOfContact</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3-0-1) |

##processStep
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **processStep** | array | A description of a non-trivial event or transformation taken to prepare the source data for use in creating the data identified by the data quality scope. |   | <ul><li>ISO 19115-2<ul><li>LI_Source &gt; sourceStep &gt; LI_ProcessStep</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2) |
| stepId |string | Serial identifier used to order the sequence of steps used. | false | <ul><li>ISO 19115-2<ul><li>LI_ProcessStep @ id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-0) |
| description |string | Description of the process or methodology step. | true | <ul><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; description</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; procdesc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-1) |
| rationale |string | Requirement or purpose for the process or methodology step. | false | <ul><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; rationale</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-2) |
| dateTime |string | Date and time or date at which the process or methodology step occurred. | false | <ul><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; dateTime</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; procdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-3) |
| processor |array | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. | false | <ul><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; processor &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; proccont &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-4) |

##processingLevel
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **processingLevel** | object | Code that identifies the level of radiometric and geometric processing that has been applied. |   | <ul><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; processingLevelCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3) |
| identifier |string | A name that is used to identify the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3-1) |
| version |string | The version of the identifier. | false | <ul><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3-3) |
| type |string | The type of identifier, e.g. doi, isbn, issn, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; ISBN</li><li>CI_Citation &gt; ISSN</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3-4) |
| authority |object | Citation for the authority issuing the identifier. | false | <ul><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-3-5) |

##processor
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **processor** | array | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. |   | <ul><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; processor &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; proccont &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-4) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-4-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2-0-4-0-1) |

##properties
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **properties** | ambiguous | JSON object containing information about a feature or collection. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2) |
| includesData |boolean | A boolean indicating whether geographic object is defining an extent, or used to describe an area of exception, such as "holes" in polygons. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement &gt; EX_GeographicBoundingBox &gt; extentTypeCode</li><li>EX_Extent &gt; geographicElement &gt; EX_BoundingPolygon &gt; extentTypeCode</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-0) |
| temporalElement |object | The temporal reference associated with a feature. | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; temporalElement &gt; EX_TemporalExtent</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-1) |
| verticalElement |array | The vertical extent of the feature geometry. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-2) |
| description |string | A description of the feature. | false | <ul><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; [Point, LineString, Polygon] &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-3) |
| featureName |string | A title associated with a feature. | false | <ul><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; [Point, LineString, Polygon] &gt; name</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-4) |
| featureScope |string | A word or phrase identifying the type of object described by the feature. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-5) |
| featureAcquisitionMethod |string | Method used to establish the position of the geographic feature.  | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-6) |
| identifier |array | Identifier for the geographic element with optional cited authority. | false | <ul><li>ISO 19115-2<ul><li>geographicElement &gt; EX_GeographicDescription &gt; geographicIdentifier &gt; MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-2-3-3-0-2-0-1-7) |

##properties
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **properties** | object | An object that links to a coordinate reference system definition. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-0-0-0-2-1-1) |
| href |string | A dereferenceable URI that links to the parameters for the coordinate reference system. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-0-0-0-2-1-1-0) |
| type |string | A string that hints at the format used to represent CRS parameters at the provided URI. Suggested values are: "proj4", "ogcwkt", "esriwkt", but others can be used. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-1-0-1-0-0-0-0-2-1-1-1) |

##repository
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **repository** | object | Information about the curator or contact person and/or agency responsible for the specimens. |   | <ul><li>ISO 19115-2<ul><li>MD_Vouchers &gt; reposit &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers &gt; reposit</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4-1) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4-1-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4-1-1) |

##resourceCitation
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **resourceCitation** | object | Citation for the associated resource. |   | <ul><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref &gt; citeinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3) |
| edition |string | Version identifier for the resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-2) |
| title |string | Name by which the cited resource is known. | true | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-0) |
| alternateTitle |string | Alias by which the cited resource is known. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-1) |
| date |array | Date referenced to the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-2) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-3) |
| onlineResource |array | On-line information related to the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-3-0-0-3-0-4) |

##resourceInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **resourceInfo** | object | Information about the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_Metadata &gt; identificationInfo &gt; MD_DataIdentification</li></ul></li><li>FGDC CSDGM<ul><li>idinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| resourceType |string | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; hierarchyLevel [MD_ScopeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-0) |
| citation |object | Citation for the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; citation &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-1) |
| resourceTimePeriod |object | Time period for the resource, e.g. project start and end date(s). | false | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; temporalElement &gt; EX_TemporalExtent &gt; extent &gt; TimePeriod</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2) |
| pointOfContact |array | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; pointOfContact</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3) |
| abstract |string | Brief narrative summary of the content of the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; abstract</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; descript &gt; abstract</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-4) |
| shortAbstract |string | A short description of the resource. Max of 300 characters. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-5) |
| status |string | Status of the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; status [MD_ProgressCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; status &gt; progress</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-6) |
| hasMapLocation |boolean | A flag indicating that a resource has a geographic location associated with it and therefore can be located using a map interface. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-7) |
| hasDataAvailable |boolean | A flag to indicate whether data for this resource is available for distribution. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-8) |
| language |array | Language(s) used within the resource. Should be a valid ISO 639-3 code. NOTE:This property has been deprecated in favor of 'locale'. | true | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9) |
| characterSet |array | Full name of the character encoding standard used by the resource. NOTE:This property has been deprecated in favor of 'locale'. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-10) |
| locale |array | Localised language(s) and characterset(s) used within the resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11) |
| purpose |string | A summary of intentions for which the resource was created. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; purpose</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; descript &gt; purpose</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12) |
| credit |array | A narrative identification of additional resources credited for the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; credit</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; datacred</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13) |
| topicCategory |array | General theme keyword of the resource, such as: oceans, biota atmosphere, etc. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; topicCategory</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14) |
| environmentDescription |string | Description of the dataset in the producer's processing environment, including items such as the software, the computer, the computer operating system, file name, and the dataset size. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; environmentDescription</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; native</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15) |
| resourceNativeFormat |array | Provides a description of the format of the resource(s). | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceFormat &gt; MD_Format</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| keyword |array | Provides category keywords, their type, and reference source. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; descriptiveKeywords &gt; MD_Keywords</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; keywords</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| resourceMaintenance |array | Information about the maintenance of the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| resourceSpecificUsage |array | Description of ways in which the resource is currently or has been used. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceSpecificUsage &gt; MD_Usage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| graphicOverview |array | Provides a path or link to images, maps, flow charts, models, etc. that illustrate the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; graphicOverview &gt; MD_BrowseGraphic</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20) |
| constraint |object | Provides information about constraints to the use of the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| taxonomy |object | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; taxonomy</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22) |
| spatialReferenceSystem |object | Geospatial referencing system used in the the data resource. The reference can be provided by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. | false | <ul><li>ISO 19115-2<ul><li>MD_Metadata &gt; referenceSystemInfo &gt; MD_ReferenceSystem &gt; referenceSystemIdentifier &gt; RS_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| spatialRepresentation |array | Format of the resource geographic extent, such as: vector, grid, etc. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdenification &gt; spatialRepresentationType [MD_SpatialRepresentationTypeCode]</li></ul></li><li>FGDC CSDGM<ul><li>spdoinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24) |
| spatialResolution |array | Information about the scale of the geographic extent. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdenification &gt; spatialResolution &gt; MD_Resolution</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| extent |array | Information about the geographic, vertical, and temporal extent of the resource. A resource may have multiple extents. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; extent &gt; EX_Extent</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26) |
| gridInfo |array | Information about grid objects in the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27) |
| coverageInfo |array | Details about the content of a raster(grid) resource. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; contentInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28) |
| dataQualityInfo |array | Information that describes the data quality, lineage, and/or processing steps that were applied to the whole or part of the data resource. | false | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; dataQualityInfo &gt; DQ_DataQuality</li></ul></li><li>FGDC CSDGM<ul><li>dataqual</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29) |
| supplementalInfo |string | Any other descriptive information about the dataset. | false | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; supplementalInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-30) |

##resourceMaintenance
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **resourceMaintenance** | array | Information about the maintenance of the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| maintenanceFrequency |string | Describes the frequency of additions and updates made to a resource. | false | <ul><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceAndUpdateFrequency [MD_MaintenanceFrequencyCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-0) |
| maintenanceNote |array | Notes regarding the maintenance of the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceNote</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-1) |
| maintenanceContact |array | Contact information for the maintainer of the resource. | false | <ul><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; contact &gt; CI_Contact</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-2) |

##resourceNativeFormat
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **resourceNativeFormat** | array | Provides a description of the format of the resource(s). |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceFormat &gt; MD_Format</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| formatName |string | Name of the data transfer format. | true | <ul><li>ISO 19115-2<ul><li>MD_Format &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtinfo &gt; formname</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-0) |
| version |string | Version of the format (date, number, etc.) | false | <ul><li>ISO 19115-2<ul><li>MD_Format &gt; version</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-1) |

##resourceSpecificUsage
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **resourceSpecificUsage** | array | Description of ways in which the resource is currently or has been used. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceSpecificUsage &gt; MD_Usage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| specificUsage |string | A brief description about how the resource is being used. | true | <ul><li>ISO 19115-2<ul><li>MD_Usage &gt; specific usage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-0) |
| userDeterminedLimitation |string | A brief description of applications, determined by the user, for which the resource is not suitable. | false | <ul><li>ISO 19115-2<ul><li>MD_Usage &gt; userDeterminedLimitations</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-1) |
| userContactInfo |array | Identification of the persons and/or organizations that are using the resource. | true | <ul><li>ISO 19115-2<ul><li>MD_Usage &gt; userContactInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-2) |

##resourceTimePeriod
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **resourceTimePeriod** | object | Time period for the resource, e.g. project start and end date(s). |   | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; temporalElement &gt; EX_TemporalExtent &gt; extent &gt; TimePeriod</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2) |
| id |string | A unique identifier for a time period. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-0) |
| description |string | A brief description providing relevant information about the time period. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; description </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-1) |
| beginPosition |string | Starting date, or date and time. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; beginPosition </li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; timeperd &gt; rngdates &gt; begdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-2) |
| endPosition |string | Ending date, or date and time. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; endPosition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; timeperd &gt; rngdates &gt; enddate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2-3) |

##responsibleParty
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **responsibleParty** | array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. |   | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0-0-1-0-3-0-1) |

##schema
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **schema** | object | schema for ADIwg mdJSON metadata |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=) |
| version |object | Identifies the version of the JSON schema standard that applies to the metadata. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0) |
| contact |array | An array of contacts to be referenced throughout the metadata. Any contact used in the metadata record must be stored within this array and referenced by contactId. Items in array may be used 0-n times throughout the record. | true | <ul><li>ISO 19115-2<ul><li>Contact &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>[single member of array] = cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1) |
| metadata |object | The main body of the metadata record. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata</li></ul></li><li>FGDC CSDGM<ul><li>metadata</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2) |
| dataDictionary |array | A description of the contents, format and structure of the physical objects in a data resource. | false | <ul><li>ISO 19115-2<ul><li>FC_FeatureCatalogue</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3) |

##securityConstraint
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **securityConstraint** | array | Handling restrictions imposed on the resource or metadata for national security or similar security concerns. |   | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; resourceConstraints &gt; MD_SecurityConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2) |
| classification |string | Name of the handling restrictions on the resource or metadata. | true | <ul><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; classification [MD_ClassificationCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2-0-0) |
| userNote |string | Explanation of the application of the legal constraints or other restrictions and legal prerequisites for obtaining and using the resource or metadata. | false | <ul><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; userNote</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2-0-1) |
| classificationSystem |string | Name of the classification system associated with a security constraint. | false | <ul><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; classificationSystem</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2-0-2) |
| handlingDescription |string | Additional description regarding the security handling of the resource or metadata. | false | <ul><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; handlingDescription</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-2-0-3) |

##sensorInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **sensorInfo** | object | Information about the sensor that collected the grid cell values. |   | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmi:rangeElementDescription &#124; gmd:dimension</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-12) |
| toneGradations |integer | The number of discrete numerical values in the grid data. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:toneGradition &gt; gco:Integer</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-12-0) |
| sensorMin |number | The shortest wavelength that the sensor is capable of collecting within a designated band. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-12-1) |
| sensorMax |number | The longest wavelength that the sensor is capable of collecting within a designated band. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-12-2) |
| sensorUnits |string | The unit in which sensor wavelengths are expressed. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-12-3) |
| sensorPeakResponse |number | The wavelength at which the sensor response is highest. | false | <ul><li>ISO 19115-2<ul><li>MI_CoverageDescription &gt; gmd:dimension &gt; gmd:MD_Band &gt; gmd:peakResponse &gt; gco:Real</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-28-0-4-0-12-4) |

##source
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **source** | array | Information about the source data used in creating the data identified by the data quality scope. |   | <ul><li>ISO 19115-2<ul><li>LI_Lineage &gt; source &gt; LI_Source</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; srcinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2) |
| description |string | A brief description about the source dataset used in creating the data identified by the data quality scope. | false | <ul><li>ISO 19115-2<ul><li>LI_Source &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-0) |
| citation |object | A citation providing information about the source dataset, including an online resource or other access instructions. | false | <ul><li>ISO 19115-2<ul><li>LI_Source &gt; sourceCitation &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; srcinfo &gt; srccite &gt; citeinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-1) |
| processStep |array | A description of a non-trivial event or transformation taken to prepare the source data for use in creating the data identified by the data quality scope. | false | <ul><li>ISO 19115-2<ul><li>LI_Source &gt; sourceStep &gt; LI_ProcessStep</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-29-0-1-2-0-2) |

##spatialReferenceSystem
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **spatialReferenceSystem** | object | Geospatial referencing system used in the the data resource. The reference can be provided by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. |   | <ul><li>ISO 19115-2<ul><li>MD_Metadata &gt; referenceSystemInfo &gt; MD_ReferenceSystem &gt; referenceSystemIdentifier &gt; RS_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| name |array | A recognized reference system name. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0) |
| epsgNumber |array | The EPSG Geodetic Parameter Dataset of the reference system, see epsg-registry.org. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-1) |
| wkt |array | Well-known text representation of the reference system. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-2) |

##spatialResolution
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **spatialResolution** | array | Information about the scale of the geographic extent. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdenification &gt; spatialResolution &gt; MD_Resolution</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| equivalentScale |number | Scale of geographic extent expressed in a hardcopy map scale fraction (denominator). | true | <ul><li>ISO 19115-2<ul><li>MD_Resolution &gt; equivalentScale &gt; MD_RepresentativeFraction &gt; denominator &gt; Integer</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-0-0) |
| distance |number | Ground distance measurement representing geographic extent. | true | <ul><li>ISO 19115-2<ul><li>MD_Resolution &gt; distance &gt; Distance </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-0) |
| uom |string | Ground distance units of measure. | false | <ul><li>ISO 19115-2<ul><li>MD_Resolution &gt; distance &gt; Distance @uom</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1-1) |

##taxonClass
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **taxonClass** | array | Information about the range of taxa addressed in the data set or collection. It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division/Phylum, class, Order, Family, Genus, and Species should be included as ranks as appropriate. |   | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxonCl &gt; MD_TaxonCl</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-5) |
| taxonRank |string | Name of the taxonomic rank for which the taxonValue is provided. Example: "Kingdom", "Division", "Phylum", "Subphylum", "SuperClass", "Class", "SubClass", "InfraClass", "Superorder", "Order", "Suborder", "Infraorder", "Superfamily", "Family", "Subfamily", "Tribe", "Subtribe", "Genus", "Species". | true | <ul><li>ISO 19115-2<ul><li> MD_TaxonCl &gt; taxonrn</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; taxonrn</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-5-0-0) |
| taxonValue |string | Taxonomic rank value of the taxon being described. | true | <ul><li>ISO 19115-2<ul><li>MD_TaxonCl &gt; taxonrv</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; taxonrv</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-5-0-1) |
| common |string | Specification of applicable common names. These common names may be general descriptions of a group of organisms if appropriate (e.g. insects, vertebrate, grasses, waterfowl, vascular plants, etc.). | false | <ul><li>ISO 19115-2<ul><li>MD_TaxonCl &gt; common</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; common</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-5-0-2) |

##taxonomy
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **taxonomy** | object | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. |   | <ul><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; taxonomy</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22) |
| classificationSystem |array | Information (citation) about the taxonomic classification system or authority used. | true | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; classSys &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; classsys</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-0) |
| taxonGeneralScope |string | Description of the range of taxa addressed in the data set or collection. For example, "all vascular plants were identified to family or species, mosses and lichens were identified as moss or lichen". | false | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxongen</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-1) |
| observer |array | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. | false | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; obs &gt; CI_ResponsibleParty</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-2) |
| taxonomicProcedure |string | Description of the methods used for taxonomic identification. Could include specimen processing, comparison with museum materials, keys, and key characters, chemical or genetic analyses, etc. | true | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxonpro</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; taxonpro</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-3) |
| voucher |object | Information on the types of specimen, the repository, and the individuals who identified the vouchers. | false | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; voucher &gt; MD_Vouchers</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4) |
| taxonClass |array | Information about the range of taxa addressed in the data set or collection. It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division/Phylum, class, Order, Family, Genus, and Species should be included as ranks as appropriate. | true | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxonCl &gt; MD_TaxonCl</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-5) |

##temporalElement
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **temporalElement** | object | An array of objects each describing a temporal boundary comprising all or a portion of the resource. |   | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; temporalElement &gt; EX_TemporalExtent</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3) |
| timeInstant |array | A set of date-time instances, each with an associated identifier and description. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-0) |
| timePeriod |array | A set of time periods(a span of time represented by a starting date-time and an ending date-time). | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-1) |
| date |array | A set of date-times. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant &gt; timePosition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-2) |

##thesaurus
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **thesaurus** | object | Name of the formally registered thesaurus or a similar authoritative source of keywords. |   | <ul><li>ISO 19115-2<ul><li>MD_Keywords &gt; thesaurusName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo&gt;keywords&gt;theme&gt;themekt</li><li>idinfo&gt;keywords&gt;place&gt;placekt</li><li>idinfo&gt;keywords&gt;temporal&gt;tempkt</li><li>idinfo&gt;keywords&gt;stratum&gt;stratkt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2) |
| edition |string | Version identifier for the resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-0) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-1) |
| identifier |array | Identifier for the resource in the context of the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-2) |
| title |string | Name by which the cited resource is known. | true | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-3-0-0) |
| alternateTitle |string | Alias by which the cited resource is known. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-3-0-1) |
| date |array | Date referenced to the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-3-0-2) |
| responsibleParty |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-3-0-3) |
| onlineResource |array | On-line information related to the citation. | false | <ul><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-2-3-0-4) |

##timeInstant
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **timeInstant** | array | A set of date-time instances, each with an associated identifier and description. |   | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-0) |
| id |string | A unique identifier for the timeInstant. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-0-0-0) |
| description |string | A brief description providing relevant information about the date and time. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-0-0-1) |
| timePosition |string | An ISO 8601 date/timestamp. | true | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant &gt; timePosition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-0-0-2) |

##timePeriod
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **timePeriod** | array | A set of time periods(a span of time represented by a starting date-time and an ending date-time). |   | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-1) |
| id |string | A unique identifier for a time period. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-1-0-0) |
| description |string | A brief description providing relevant information about the time period. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; description </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-1-0-1) |
| beginPosition |string | Starting date, or date and time. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; beginPosition </li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; timeperd &gt; rngdates &gt; begdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-1-0-2) |
| endPosition |string | Ending date, or date and time. | false | <ul><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; endPosition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; timeperd &gt; rngdates &gt; enddate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-3-1-0-3) |

##userContactInfo
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **userContactInfo** | array | Identification of the persons and/or organizations that are using the resource. |   | <ul><li>ISO 19115-2<ul><li>MD_Usage &gt; userContactInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-2-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-2-0-1) |

##version
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **version** | object | Identifies the version of the JSON schema standard that applies to the metadata. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0) |
| name |string | Schema identifier, i.e. the name of the schema standard. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-0) |
| version |string | Specific version number of the schema standard. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-1) |

##verticalElement
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **verticalElement** | array | An array of objects each describing a vertical boundary comprising all or a portion of the resource. |   | <ul><li>ISO 19115-2<ul><li>EX_Extent &gt; verticalElement &gt; EX_VerticalExtent </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-2) |
| minimumValue |number | Lowest vertical extent contained in the dataset. | true | <ul><li>ISO 19115-2<ul><li>EX_VerticalExtent &gt; minimumValue &gt; Real </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-2-0-0) |
| maximumValue |number | Highest vertical extent contained in the dataset. | true | <ul><li>ISO 19115-2<ul><li>EX_VerticalExtent &gt; maximumValue &gt; Real </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-2-0-1) |
| verticalCRSTitle |string | Name of a geographic reference system associated with a vertical extent. | true | <ul><li>ISO 19115-2<ul><li>EX_VerticalExtent &gt; verticalCRS @xlink:title </li></ul></li><li>FGDC CSDGM<ul><li>spref &gt; vertdef &gt; altsys &gt; altdatum</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-2-0-2) |
| verticalCRSUri |string | Web link to the parameters for a geographic reference system associated with a vertical extent. | true | <ul><li>ISO 19115-2<ul><li>EX_VerticalExtent &gt; verticalCRS @xlink:href </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26-0-2-0-3) |

##voucher
| Name | Type | Description | Required | Translation | Viewer Link|
|---|---|---|---|---|
| **voucher** | object | Information on the types of specimen, the repository, and the individuals who identified the vouchers. |   | <ul><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; voucher &gt; MD_Vouchers</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4) |
| specimen |string | Word or phrase describing the type of specimen collected (e.g. 'herbarium specimens', 'blood samples', 'photographs', 'individuals', or 'batches'). | true | <ul><li>ISO 19115-2<ul><li>MD_Vouchers &gt; specimen</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers &gt; specimens</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4-0) |
| repository |object | Information about the curator or contact person and/or agency responsible for the specimens. | true | <ul><li>ISO 19115-2<ul><li>MD_Vouchers &gt; reposit &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers &gt; reposit</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4-1) |