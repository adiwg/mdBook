# mdJSON v2.3.2 Data Dictionary

<!-- toc -->

## additionalDocumentation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **additionalDocumentation** | array | Other documents related to, but not defining, the resource such as factsheets, data catalog pages, award documents, proposals, and informational websites. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5) |
| [resourceType](#resourcetype) |array | Identifies the type of resource, such as: userGuide, website, report, etc. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>[MD_ScopeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-0) |
| [citation](#citation) |array | Citation for the additional resource. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1) |

## address
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **address** | array | Addresses for this contact. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7) |
| addressType |array | The type of address, usually mailing and/or physical. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7-0-0) |
| description |string | Description of the address. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7-0-1) |
| deliveryPoint |array | Address line for the location. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Address &gt; deliveryPoint</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; address</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7-0-2) |
| city |string | City of the location. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Address &gt; city</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; city</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7-0-3) |
| administrativeArea |string | State, province of the location. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Address &gt; administrativeArea</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; state</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7-0-4) |
| postalCode |string | ZIP or other postal code. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Address &gt; postalCode</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; postal</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7-0-5) |
| country |string | ZIP or other postal code. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Address &gt; postalCode</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntaddr &gt; postal</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7-0-6) |

## addressee
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **addressee** | array | undefined |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5-0) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5-0-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5-0-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5-0-0-2) |

## allocation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **allocation** | array | Funds contributed to support the development of the resource. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0) |
| amount |number | The amount of the allocation in the indicated currency. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0-0-0) |
| currency |string | The ISO 4217 currency code. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0-0-1) |
| sourceId |string | The contactId of the entity providing the allocation. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0-0-2) |
| recipientId |string | The contactId of the entity receiving the allocation. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0-0-3) |
| matching |boolean | Indicates whether the funds are to be considered matching funds. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0-0-4) |
| comment |string | Additional information relevant to the allocation. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0-0-5) |

## alternateMetadataReference
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **alternateMetadataReference** | array | Reference to alternative metadata for the resource. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7-0-10) |

## associatedResource
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **associatedResource** | array | Other resources which are directly related to the subject resource such as parent, child, or sibling datasets or projects. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |
| associationType |string | Identifies how the associated resource is related to the subject resource such as 'is a component of', 'larger work citation', 'cross reference', etc. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; associationType [DS_AssociationTypeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-0) |
| initiativeType |string | Identifies type of initiative under which the resource was produced - the activity that resulted in the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; initiativeType &gt; [DS_InitiativeTypeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-1) |
| [resourceType](#resourcetype) |array | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>[MD_ScopeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-2) |
| [resourceCitation](#resourcecitation) |object | Citation for the associated resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref &gt; citeinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3) |
| [metadataCitation](#metadatacitation) |object | Citation for the associated resource metadata. | false | <ul class="md-translation"><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo</li></ul></li><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4) |

## attributeGroup
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **attributeGroup** | array | Information about groups of attributes describing a coverage. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3) |
| attributeContentType |array | Type of information represented by the values | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &#124; MI_CoverageDescription &gt; contentType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-0) |
| [attribute](#attribute) |array |  | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-1) |

## attributeIdentifier
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **attributeIdentifier** | array | Identifiers for each attribute included in the resource. NOTE: These identifiers can be used to provide names for the attribute from a standard set of names. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-1-0-3) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-1-0-3-0-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-1-0-3-0-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-1-0-3-0-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-1-0-3-0-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3-0-1-0-3-0-4) |

## attribute
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **attribute** | array | An array of objects defining the attributes for the entity |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7) |
| commonName |string | The common name used to identify this attribute | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; memberName &gt; localName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-0) |
| codeName |string | The code used to identify this attribute.  Most often this will be the table or spreadsheet column name | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; code &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-1) |
| alias |array | An array of quoted strings providing alternate names by which the attribute is known | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-2) |
| definition |string | A succinct but comprehensive definition for the attribute | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; definition &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-3) |
| dataType |string | The datatype for the attribute.  Names for datatypes vary widely by database management system.  Use the datatype name associated with the database system that implemented the entity.  E.g. 'integer', 'boolean', 'decimal(8,5)', 'varchar(200)' | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; valueType &gt; TypeName &gt; aName &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-4) |
| allowNull |boolean | Indicates whether null values are allowed for the attribute | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; cardinality &gt; Multiplicity &gt; range &gt; MultiplicityRange &gt; lower &gt; integer[0=optional &#124; 1=required]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-5) |
| allowMany |boolean | Indicates whether null values are allowed for the attribute | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-6) |
| units |string | A unit-of-measure for the attribute.  E.g. 'meters', 'atmospheres', 'liters' | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; valueMeasurementUnit &gt; [UnitDefinition &gt; identifier &#124; ConversionalUnit &gt; identifier, name, catalogSystem, conversionToPreferredUnit, formula &#124; BaseUnit &gt; identifier, name, catalogSymbol, unitSystem &#124; DerivedUnit &gt; identifier, name, remarks, catalogSymbol, derivationUnitTerm]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-7) |
| domainId |string | Provides the domain ID for the  dictionary Domain containing the list of permissable values for this attribute | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-8) |
| minValue |string | The minimum range value permissible for this attribute | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-9) |
| maxValue |string | The maximum range value permissible for this attribute | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7-0-10) |

## authority
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **authority** | object | Citation for the authority issuing the identifier. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4-10) |

## boundingBox
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **boundingBox** | object | General geographic position of the resource. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-2) |
| westLongitude |number |  | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-2-0) |
| eastLongitude |number |  | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-2-1) |
| southLatitude |number |  | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-2-2) |
| northLatitude |number |  | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-2-3) |

## citation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **citation** | array | Citation for the additional resource. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-1-0-10) |

## citation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **citation** | object | Citation for the dictionary. |   | <ul class="md-translation"><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo</li></ul></li><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0-10) |

## constraint
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **constraint** | array | Provides information about constraints to the use of the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22) |
| type |enum: legal | Indicates the type of constraint. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-9-2-0) |
| useLimitation |array | Limitation affecting the fitness for use of the resource or metadata. For example, "not to be used for navigation". | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Constraints &gt; useLimitation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-1) |
| [scope](#scope) |object | temporal extent and or level of the application of the constraint restrictions. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-2) |
| [graphic](#graphic) |array | Graphic or symbol indicating the constraint | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-3) |
| [reference](#reference) |array | Citation for the limitation or constraint | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-4) |
| [releasability](#releasability) |object | Information concerning the parties to who the resource can or cannot be released. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-5) |
| [responsibleParty](#responsibleparty) |array | Entity responsible for the resource constraint | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-6) |
| [legal](#legal) |object | Restrictions and legal prerequisites for accessing and using the resource or metadata. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_LegalConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-7) |
| [security](#security) |object | Handling restrictions imposed on the resource or metadata for national security or similar security concerns. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_SecurityConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22-8) |

## contact
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **contact** | array | Contact information for the maintainer of the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; contact &gt; CI_Contact</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-4) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-4-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-4-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-4-0-2) |

## contact
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **contact** | array | An array of contacts to be referenced throughout the metadata. Any contact used in the metadata record must be stored within this array and referenced by contactId. Items in array may be used 0-n times throughout the record. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1) |
| contactId |string | Unique identifier for the contact. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-0) |
| isOrganization |enum: false | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-13-1-0) |
| name |string |  | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; individualName</li><li>CI_ResponsibleParty &gt; organisationName</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntperp &gt; cntper</li><li>cntinfo &gt; cntperp &gt; cntorg</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-2) |
| positionName |string | Role or position of the person, usually within a given organization. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; positionName</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-3) |
| memberOfOrganization |array | Organizations that this contact is related to. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-4) |
| [logoGraphic](#logographic) |array | Logo for contact. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li></li></ul></li><li>FGDC CSDGM<ul><li></li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-5) |
| [phone](#phone) |array | Supplemental instructions on how or when to contact the individual or organization. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Contact &gt; contactInstructions</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntinst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-6) |
| [address](#address) |array | Addresses for this contact. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-7) |
| electronicMailAddress |array | E-mail or electronic mailbox address. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Address &gt; electronicMailAddress</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntemail</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-8) |
| [onlineResource](#onlineresource) |array | Information about accessing on-line resources and services. This may be a website, profile page, GitHub page, etc. related to the contact. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_ResponsibleParty &gt; contactInfo &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-9) |
| hoursOfService |array |  | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-10) |
| contactInstructions |string | Supplemental instructions on how or when to contact the individual or organization. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Contact &gt; contactInstructions</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntinst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-11) |
| contactType |string | User defined contact type. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-12) |

## contact
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **contact** | object | Party from whom the resource may be obtained. Note: This list need not be exhaustive. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorContact &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; distrib &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-0) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-0-2) |

## cornerPoints
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **cornerPoints** | ambiguous | The earth location in the coordinate system defined by the Spatial Reference System and the grid coordinate of the cells at opposite ends of grid coverage along two diagonals in the grid spatial dimensions. Note: There are four corner points in a georectified grid; at least two corner points along one diagonal are required. The first corner point corresponds to the origin of the grid. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-3) |

## coverageDescription
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **coverageDescription** | array | Details about the content of a raster(grid) resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; contentInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| coverageName |string | The name(title) of the coverage. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &#124; MI_CoverageDescription &gt; attributeDescription &gt; gco:RecordType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-0) |
| coverageDescription |string | A description of the coverage | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &#124; MI_CoverageDescription &gt; attributeDescription &gt; gco:RecordType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-1) |
| [processingLevelCode](#processinglevelcode) |object | Code that identifies the level of radiometric and geometric processing that has been applied. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; processingLevelCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2) |
| [attributeGroup](#attributegroup) |array | Information about groups of attributes describing a coverage. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-3) |
| [imageDescription](#imagedescription) |object | Information about an image's suitability for use. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4) |

## crsId
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **crsId** | object | Identifies the vertical coordinate reference system used for the minimum and maximum values. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Metadata &gt; referenceSystemInfo &gt; MD_ReferenceSystem &gt; referenceSystemIdentifier &gt; RS_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-2-0-2-0-3) |

## dataDictionary
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **dataDictionary** | array | A description of the contents, format and structure of the physical objects in a data resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4) |
| [citation](#citation) |object | Citation for the dictionary. | true | <ul class="md-translation"><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo</li></ul></li><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-0) |
| subject |array | Identifies the scope of the data dictionary. E.g. 'database', 'dataset', 'table'. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; scope</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-1) |
| recommendedUse |array | Description of kind(s) of use to which this dictionary may be put. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; fieldOfApplication &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-2) |
| [locale](#locale) |array | Defines the language and country of origin in which the data dictionary is written.  E.g. 'eng; USA', 'eng; UK', 'esp; MEX'. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-3) |
| [responsibleParty](#responsibleparty) |object | Name, address, country, and telecommunications address of person or organization having primary responsibility for the intellectual content of this dictionary. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4) |
| dictionaryFormat |string | Formal functional language used in the dictionary. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-5) |
| dictionaryIncludedWithResource |boolean | Indication of whether or not the data dictionary is included with the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_FeatureCatalogueDescription &gt; includedWithDataset</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-6) |
| [domain](#domain) |array | A list of permissable values used to constrain an attribute's value.  A single domain may be assigned to multiple attributes in a table or database. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7) |
| [entity](#entity) |array | Defines the structure of a discrete data object within the data resource.  The data object may be a table, dataset, or single sheet of a spreadsheet. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8) |

## date
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **date** | array | Date referenced to the cited resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-2) |
| date |string | An ISO 8601 date/timestamp. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Date &gt; date</li><li>FC_FeatureCatalogue &gt; versionDate</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; pubdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-2-0-0) |
| dateType |string | The type of date. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Date &gt; dateType [CI_DateTypeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-2-0-1) |
| description |string | Supplemental information describing the date context. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-2-0-2) |

## defaultMetadataLocale
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **defaultMetadataLocale** | object | Main localised language and characterset used within the metadata record. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| language |string | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-0) |
| characterSet |string | Full name of the character encoding standard used by the resource(see http://www.iana.org/assignments/character-sets/character-sets.xhtml). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-1) |
| country |string | Designation of the specific country of the locale language(ISO 3166-1). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2-2) |

## defaultResourceLocale
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **defaultResourceLocale** | object | Localised language(s) and characterset(s) used within the resource. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| language |string | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-0) |
| characterSet |string | Full name of the character encoding standard used by the resource(see http://www.iana.org/assignments/character-sets/character-sets.xhtml). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-1) |
| country |string | Designation of the specific country of the locale language(ISO 3166-1). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23-2) |

## dimension
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **dimension** | array | Information about spatial-temporal axis properties. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1) |
| dimensionType |string | The type of dimension for this axis. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; dimensionName &gt; MD_DimensionNameTypeCode</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-0) |
| dimensionSize |integer | The number of elements along the axis. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; dimensionSize</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-1) |
| [resolution](#resolution) |object | The degree of detail in the grid. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; resolution</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-2) |
| dimensionTitle |string | The name of the axis. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li></li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-3) |
| dimensionDescription |string | The description of the axis. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li></li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-4) |

## distributionFormat
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **distributionFormat** | array | Provides information about the format used by the distributor. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorFormat &gt; MD_Format</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5) |
| [formatSpecification](#formatspecification) |object | Citation of the specification for the format. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Format &gt; name</li><li>MD_Format &gt; version</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtinfo &gt; formname</li><li>idinfo &gt; citation &gt; citeinfo &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0) |
| amendmentNumber |string | Amendment number of the format version. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-1) |
| compressionMethod |string | Recommendations of algorithms or processes that can be applied to read or expand resources to which compression techniques have been applied. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-2) |

## distributor
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **distributor** | array | Information about the distributor of and options for obtaining the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution</li></ul></li><li>FGDC CSDGM<ul><li>distinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1) |
| [contact](#contact) |object | Party from whom the resource may be obtained. Note: This list need not be exhaustive. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorContact &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; distrib &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-0) |
| [orderProcess](#orderprocess) |array | Provides information about how the resource may be obtained and related instructions and fee information. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributionOrderProcess</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-1) |
| [transferOption](#transferoption) |array | Describes method and media by which a resource is obtained from the distributor. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distributor &gt; distributorTransferOptions</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2) |

## documentedIssue
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **documentedIssue** | object | Citation of a description of known issues associated with the resource along with proposed solutions if available. |   | <ul class="md-translation"><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo</li></ul></li><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4-10) |

## domainItem
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **domainItem** | array | An array of member objects that enumerate and define the valid values for a domain. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-4) |
| name |string | A descriptive name associated with a domain value | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; listedValue &gt; FC_ListedValue &gt; label</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-4-0-0) |
| value |string | A descriptive name associated with a domain value | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; listedValue &gt; FC_ListedValue &gt; label</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-4-0-1) |
| definition |string | A brief definition for the domain item | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute &gt; listedValue &gt; FC_ListedValue &gt; definition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-4-0-2) |

## domain
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **domain** | array | A list of permissable values used to constrain an attribute's value.  A single domain may be assigned to multiple attributes in a table or database. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7) |
| domainId |string | A user provided unique ID for this domain.  The ID will be used to locate the domain in the domain array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-0) |
| commonName |string | A short common name for the domain. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-1) |
| codeName |string | The code or 'lookup table' name for the domin used in the database schema definitions. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-2) |
| description |string | A brief description of the domain including identification of any established sources used in creating the list of domain items. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-3) |
| [domainItem](#domainitem) |array | An array of member objects that enumerate and define the valid values for a domain. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-7-0-4) |

## duration
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **duration** | object | Object for collecting information about a duration or period of time. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-7) |
| years |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-7-0) |
| months |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-7-1) |
| days |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-7-2) |
| hours |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-7-3) |
| minutes |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-7-4) |
| seconds |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-7-5) |

## entity
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **entity** | array | Defines the structure of a discrete data object within the data resource.  The data object may be a table, dataset, or single sheet of a spreadsheet. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8) |
| entityId |string | A user provided unique ID for this entity.   | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType#id=''</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-0) |
| commonName |string | The name commonly used to identify this entity | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; typeName &gt; localName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-1) |
| codeName |string | The code name used to identify this entity in a database schema or application software. For spreasheets this would likely be the sheet name.  | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; code &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-2) |
| alias |array | An array of quoted strings providing alternate names used to identify this entity | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; aliases &gt; localName</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-3) |
| definition |string | A brief definition for the entity | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; definition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-4) |
| primaryKeyAttributeCodeName |array | An array of quoted attribute code names that together compose the primary key set for the entity | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>Note: the primary key is written as a text description into FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-5) |
| [index](#index) |array | An array of objects describing alternate indexes for the entity | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; Note: the index is written as a text description into featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-6) |
| [attribute](#attribute) |array | An array of objects defining the attributes for the entity | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; carrierOfCharacteristics &gt; FC_FeatureAttribute</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-7) |
| [foreignKey](#foreignkey) |array | An array of objects describing attributes whose values are restricted to values found in the domain of an attribute belonging to another table or dataset | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>Note: the foreign key is written as a text description into FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-8) |

## extent
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **extent** | array | Information about the geographic, vertical, and temporal extent of the resource. A resource may have multiple extents. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; extent &gt; EX_Extent</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15) |
| description |string | Description of the extent. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-0) |
| [geographicExtent](#geographicextent) |array | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-1) |
| [verticalExtent](#verticalextent) |array | An array of objects each describing a vertical boundary comprising all or a portion of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; verticalElement &gt; EX_VerticalExtent </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-2) |
| [temporalExtent](#temporalextent) |array | An array of objects each describing a temporal boundary comprising all or a portion of the resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15-0-3) |

## features
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **features** | array | Set of Features constituting the FeatureCollection. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; MultiGeometry</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-1-0-3-0-1-0-1-3-1) |
| type |enum: Feature | Type of GeoJSON object. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-1-0-3-0-1-0-1-3-1-0-0) |
| geometry |ambiguous | The geometry object associated with the Feature. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-1-0-3-0-1-0-1-3-1-0-1) |
| [properties](#properties) |ambiguous | JSON object containing information about a feature or collection. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-1-0-3-0-1-0-1-3-1-0-2) |
| id |string,number | Unique identifier for the GeoJSON feature object. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>geographicElement &gt; EX_BoundingPolygon &gt; polygon &gt; [Point, LineString, Polygon] @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-1-0-3-0-1-0-1-3-1-0-3) |

## fileConstraint
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **fileConstraint** | array | Identifies, legal, security, and other constraint requirements associated with use and distribution of the graphic |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10-0-3) |
| type |enum: legal | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-9-2-0) |

## fileUri
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **fileUri** | array | URI of the graphic. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename @xlink:href</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-4) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; linkage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-4-0-0) |
| name |string | Name of the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; name</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-4-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; protocol</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-4-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-4-0-3) |
| function |string | Function performed by the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; function &gt; CI_OnlineFunctionCode [codelist]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-4-0-4) |

## foreignKey
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **foreignKey** | array | An array of objects describing attributes whose values are restricted to values found in the domain of an attribute belonging to another table or dataset |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>Note: the foreign key is written as a text description into FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-8) |
| localAttributeCodeName |array | An array of local (referencing or child) attribute code names for this foreign key | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-8-0-0) |
| referencedEntityCodeName |string | The entityID for the referenced (or parent) entity for this foreign key | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-8-0-1) |
| referencedAttributeCodeName |array | An array of referenced (or parent) attribute code names for this foreign key.  If the foreign key is compound key (more than one attribute compose the key) the order of the referenced attributes must allign precicely with the order and number of local attributes. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-8-0-2) |

## formatSpecification
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **formatSpecification** | object | Citation of the specification for the format. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Format &gt; name</li><li>MD_Format &gt; version</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtinfo &gt; formname</li><li>idinfo &gt; citation &gt; citeinfo &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5-0-0-10) |

## funding
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **funding** | array | Information about funding for the resource. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6) |
| [allocation](#allocation) |array | Funds contributed to support the development of the resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-0) |
| [timePeriod](#timeperiod) |object | The period for which the allocation is relevant. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6-0-1) |

## geographicElement
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **geographicElement** | array | An array of objects each describing a geographic boundary or location comprising all or a portion of the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-3) |
| type |enum: Feature, FeatureCollection, GeometryCollection, Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon | The type of geographic object. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-3-0-0) |
| bbox |array | A GeoJSON object MAY have a member named 'bbox' to include information on the coordinate range for its Geometries, Features, or FeatureCollections. The value of the bbox member MUST be an array of length 2 * n where n is the number of dimensions represented in the contained geometries, with all axes of the most southwesterly point followed by all axes of the more northeasterly point. The axes order of a bbox follows the axes order of geometries. The values of a 'bbox' array are[west, south, east, north]. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; geographicElement &gt; EX_GeographicBoundingBox, EX_GeographicBoundingBox &gt; westBoundLongitude &gt; Decimal {west}, EX_GeographicBoundingBox &gt; eastBoundLongitude &gt; Decimal {east}, EX_GeographicBoundingBox &gt; southBoundLatitude &gt; Decimal {south}, EX_GeographicBoundingBox &gt; northBoundLatitude &gt; Decimal {north}</li></ul></li><li>FGDC CSDGM<ul><li>[idinfo &gt; spdom &gt; bounding &gt; westbc], [idinfo &gt; spdom &gt; bounding &gt; eastbc], [idinfo &gt; spdom &gt; bounding &gt; northbc], [idinfo &gt; spdom &gt; bounding &gt; southbc]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-1-0-3-0-1-0-0) |

## geographicExtent
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **geographicExtent** | array | undefined |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1-0-1) |

## georectifiedRepresentation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **georectifiedRepresentation** | object | A grid whose cells are regularly spaced in a geographic (i.e. lat/long) or map coordinate system defined in the SpatialReferencing System (SRS) so that any cell in the grid can be geolocated given its grid coordinates and the grid origin, cell spacing, and orientation. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0) |
| [gridRepresentation](#gridrepresentation) |object | Information about grid objects in the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-0) |
| checkPointAvailable |boolean | Idication of whether or not geographic position points are available to test the accuracy of the georeferenced grid data. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-1) |
| checkPointDescription |string | Description of geographic positions points used to test the accuracy of the georeferenced grid data. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-2) |
| [cornerPoints](#cornerpoints) |ambiguous | The earth location in the coordinate system defined by the Spatial Reference System and the grid coordinate of the cells at opposite ends of grid coverage along two diagonals in the grid spatial dimensions. Note: There are four corner points in a georectified grid; at least two corner points along one diagonal are required. The first corner point corresponds to the origin of the grid. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-3) |
| centerPoint |array | The earth location in the coordinate system defined by the Spatial Reference System and the grid coordinate of the cell halfway between opposite ends of the grid in the spatial dimensions. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-4) |
| pointInPixel |string | Point in a pixel corresponding to the Earth location of the pixel. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-5) |
| transformationDimensionDescription |string | Point in a pixel corresponding to the Earth location of the pixel. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-6) |
| transformationDimensionMapping |string | Point in a pixel corresponding to the Earth location of the pixel. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0-7) |

## georeferenceableRepresentation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **georeferenceableRepresentation** | object | Grid with cells irregularly spaced in any given geographic/map projection coordinate system, whose individual cells can be geolocated using geolocation information supplied with the data but cannot be geolocated from the grid properties alone. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0) |
| [gridRepresentation](#gridrepresentation) |object | Information about grid objects in the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0) |
| controlPointAvailable |boolean | Indication of whether or not control point(s) exist. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-1) |
| orientationParameterAvailable |boolean | Description of the parameters used to describe sensor orientation. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-2) |
| orientationParameterDescription |string | Description of parameters used to describe sensor orientation. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-3) |
| georeferencedParameter |string | Information which support grid data georeferencing. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-4) |
| [parameterCitation](#parametercitation) |array | Reference providing description of the parameters. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5) |

## graphicOverview
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **graphicOverview** | array | Provides a path or link to images, maps, flow charts, models, etc. that illustrate the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; graphicOverview &gt; MD_BrowseGraphic</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| fileName |string | Name of the file that contains a graphic describing the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsen</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-0) |
| fileDescription |string | Description of the graphic. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileDescription</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsed</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-1) |
| fileType |string | The format in which the illustration is encoded such as GIF, JPEG, PBM, PS, TIFF. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileType</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browset</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-2) |
| [fileConstraint](#fileconstraint) |array | Identifies, legal, security, and other constraint requirements associated with use and distribution of the graphic | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-3) |
| [fileUri](#fileuri) |array | URI of the graphic. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename @xlink:href</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18-0-4) |

## graphic
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **graphic** | array | Online graphic associated with the citation |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10) |
| fileName |string | Name of the file that contains a graphic describing the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsen</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10-0-0) |
| fileDescription |string | Description of the graphic. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileDescription</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsed</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10-0-1) |
| fileType |string | The format in which the illustration is encoded such as GIF, JPEG, PBM, PS, TIFF. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileType</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browset</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10-0-2) |
| [fileConstraint](#fileconstraint) |array | Identifies, legal, security, and other constraint requirements associated with use and distribution of the graphic | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10-0-3) |
| [fileUri](#fileuri) |array | URI of the graphic. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename @xlink:href</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10-0-4) |

## gridRepresentation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **gridRepresentation** | object | Information about grid objects in the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0) |
| numberOfDimensions |number | The number of independent spatial-temporal axes. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; numberOfDimensions</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-0) |
| [dimension](#dimension) |array | Information about spatial-temporal axis properties. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1) |
| cellGeometry |string | Identification of grid data as point or cell. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; cellGeometry</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-2) |
| transformationParameterAvailable |boolean | An indication of whether or not parameters for transformation between image coordinates and geographic or map coordinates exist (are available). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; transformationParameterAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-3) |

## identificationReference
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **identificationReference** | array | Information on any non-authoritative materials (e.g. field guides) useful for reconstructing the actual process. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-2) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-2-0-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-2-0-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-2-0-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-2-0-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-2-0-4) |

## identifier
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **identifier** | array | Identifier for the resource in the context of the citation. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6-0-4) |

## identifier
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **identifier** | object | Identifier for the timePeriod. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-2) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-2-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-2-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-2-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-2-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-2-4) |

## imageDescription
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **imageDescription** | object | Information about an image's suitability for use. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4) |
| illuminationElevationAngle |number | Illumination elevation measured in degrees clockwise from the target plane at intersection of the optical line of sight with the Earth’s surface. For images from a scanning device, refer to the centre pixel of the image. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; illiminationElevationAngle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-0) |
| illuminationAzimuthAngle |number | Illumination azimuth measured in degrees clockwise from true north at the time the image is taken. For images from a scanning device, refer to the centre pixel of the image | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; illuminationAzimuthAngle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-1) |
| imagingCondition |string | Code which indicates conditions which may affect the image. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; imageCondition &gt; MD_ImageConditionCode</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-2) |
| [imageQualityCode](#imagequalitycode) |object | Specifies the image quality. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; imageQualityCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-3) |
| cloudCoverPercent |number | Area of the dataset obscured by clouds, expressed as a percentage of the spatial extent. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; cloudCoverPercentage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-4) |
| compressionQuantity |number | Count of the number of lossy compression cycles performed on the image. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; compressionGenerationQuality</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-5) |
| triangulationIndicator |boolean | Indication of whether or not triangulation has been performed upon the image. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; triangulationIndicator</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-6) |
| radiometricCalibrationAvailable |boolean | Indication of whether or not the radiometric calibration information for generating the radiometrically calibrated standard data product is available. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; radiometricCalibrationDataAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-7) |
| cameraCalibrationAvailable |boolean | Indication of whether or not constants are available which allow for camera calibration corrections. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; camerCalibrationInformationAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-8) |
| filmDistortionAvailable |boolean | Indication of whether or not Calibration Reseau information is available | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; filmDistrotionInformationAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-9) |
| lensDistortionAvailable |boolean | Indication of whether or not lens aberration correction information is available. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; lensDistortionInformationAvailability</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-10) |

## imageQualityCode
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **imageQualityCode** | object | Specifies the image quality. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; imageQualityCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-3) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-3-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-3-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-3-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-3-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-4-3-4) |

## index
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **index** | array | An array of objects describing alternate indexes for the entity |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; Note: the index is written as a text description into featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-6) |
| codeName |string | The code name used to define the alternate index on the entity | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-6-0-0) |
| allowDuplicates |boolean | Indicates whether the index allows duplicates or values are required to be unique.  true = allow duplicates; false = values must be unique. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-6-0-1) |
| attributeCodeName |array | An array of quoted attribute code names that together compose an alternate key set for the entity | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; featureType &gt; FC_FeatureType &gt; constrainedBy &gt; FC_Constraint &gt; description &gt; CharacterString</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-8-0-6-0-2) |

## keyword
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **keyword** | array | Array of ISO Topic Category keywords. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Keywords &gt; keyword</li></ul></li><li>FGDC CSDGM<ul><li>idinfo&gt;keywords&gt;theme&gt;themekey</li><li>idinfo&gt;keywords&gt;place&gt;placekey</li><li>idinfo&gt;keywords&gt;temporal&gt;tempkey</li><li>idinfo&gt;keywords&gt;stratum&gt;stratkey</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-3-0-1) |
| keyword |string | Commonly used word(s) or formalized word(s) or phrase(s) used to describe the subject. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-3-0-1-0-1-0-0) |
| keywordId |string | Identifier for the keyword. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-3-0-1-0-1-0-1) |
| keywordType |ambiguous | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-3-1-0) |

## legal
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **legal** | object | Restrictions and legal prerequisites for accessing and using the resource or metadata. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_LegalConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-7) |
| accessConstraint |array | Access constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations on obtaining the resource or metadata. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_LegalConstraints &gt; accessConstraints [MD_RestrictionCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; accconst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-7-0) |
| useConstraint |array | Constraints applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations or warnings on using the resource or metadata. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_LegalConstraints &gt; useConstraints [MD_RestrictionCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; useconst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-7-1) |
| otherConstraint |array | Other restrictions and legal prerequisites for accessing and using the resource or metadata. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_LegalConstraints &gt; otherConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-7-2) |

## locale
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **locale** | array | Defines the language and country of origin in which the data dictionary is written.  E.g. 'eng; USA', 'eng; UK', 'esp; MEX'. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>FC_FeatureCatalogue &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-3) |
| language |string | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-3-0-0) |
| characterSet |string | Full name of the character encoding standard used by the resource(see http://www.iana.org/assignments/character-sets/character-sets.xhtml). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-3-0-1) |
| country |string | Designation of the specific country of the locale language(ISO 3166-1). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-3-0-2) |

## logoGraphic
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **logoGraphic** | array | Logo for contact. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li></li></ul></li><li>FGDC CSDGM<ul><li></li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-5) |
| fileName |string | Name of the file that contains a graphic describing the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsen</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-5-0-0) |
| fileDescription |string | Description of the graphic. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileDescription</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browsed</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-5-0-1) |
| fileType |string | The format in which the illustration is encoded such as GIF, JPEG, PBM, PS, TIFF. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; fileType</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; browse &gt; browset</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-5-0-2) |
| [fileConstraint](#fileconstraint) |array | Identifies, legal, security, and other constraint requirements associated with use and distribution of the graphic | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-5-0-3) |
| [fileUri](#fileuri) |array | URI of the graphic. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_BrowseGraphic &gt; filename @xlink:href</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-5-0-4) |

## measure
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **measure** | object | Scale of geographic extent expressed in ground distance parameters or angle. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3-0-1-0) |
| type |enum: distance, length, angle, measure, scale | The type of measurement. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3-0-1-0-0) |
| value |number | The number of units in the measurement. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3-0-1-0-1) |
| unitOfMeasure |string | The type of units to associated with the value. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3-0-1-0-2) |

## mediumSpecification
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **mediumSpecification** | object | Name of the formaton which the resource may be stored |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Medium &gt; name [MD_MediumNameCode]</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn &gt; offmedia</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0-10) |

## metadataCitation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataCitation** | array | Citation providing information about the metadata for the source. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2-0-10) |

## metadataCitation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataCitation** | object | Citation for the associated resource metadata. |   | <ul class="md-translation"><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo</li></ul></li><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-4-10) |

## metadataContact
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataContact** | array | Person or organization responsible for metadata information (metadata custodian). |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; contact &gt; CI_Contact &gt; responsibleParty &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4-0-2) |

## metadataDate
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataDate** | array | Date that the metadata was updated. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; dateStamp</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metrd</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5) |
| date |string | An ISO 8601 date/timestamp. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Date &gt; date</li><li>FC_FeatureCatalogue &gt; versionDate</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; pubdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5-0-0) |
| dateType |string | The type of date. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Date &gt; dateType [CI_DateTypeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5-0-1) |
| description |string | Supplemental information describing the date context. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5-0-2) |

## metadataIdentifier
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataIdentifier** | object | Identifier for the metadata. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; fileIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0-4) |

## metadataInfo
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataInfo** | object | General information about the metadata record. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| [metadataIdentifier](#metadataidentifier) |object | Identifier for the metadata. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; fileIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-0) |
| [parentMetadata](#parentmetadata) |object | Identifier of the metadata to which this metadata is a subset (child). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; parentIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| [defaultMetadataLocale](#defaultmetadatalocale) |object | Main localised language and characterset used within the metadata record. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-2) |
| [otherMetadataLocale](#othermetadatalocale) |array | Additional localised language(s) and characterset(s) used within the metadata record. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3) |
| [metadataContact](#metadatacontact) |array | Person or organization responsible for metadata information (metadata custodian). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; contact &gt; CI_Contact &gt; responsibleParty &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-4) |
| [metadataDate](#metadatadate) |array | Date that the metadata was updated. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; dateStamp</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metrd</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-5) |
| [metadataOnlineResource](#metadataonlineresource) |array | Online location where the metadata is available. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6) |
| [alternateMetadataReference](#alternatemetadatareference) |array | Reference to alternative metadata for the resource. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-7) |
| metadataStatus |string | Status of the metadata record. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-8) |
| [metadataMaintenance](#metadatamaintenance) |object | Provides information about the frequency of metadata updates, and the scope of those updates. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; metadataMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9) |

## metadataMaintenance
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataMaintenance** | object | Provides information about the frequency of metadata updates, and the scope of those updates. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; metadataMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9) |
| frequency |string | Describes the frequency of additions and updates made to a resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceAndUpdateFrequency [MD_MaintenanceFrequencyCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-0) |
| [date](#date) |array | Date related to resource maintenance. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-1) |
| [scope](#scope) |array | Type of resource to which the maintenance information applies. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-2) |
| note |array | Notes regarding the maintenance of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceNote</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-3) |
| [contact](#contact) |array | Contact information for the maintainer of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; contact &gt; CI_Contact</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-9-4) |

## metadataOnlineResource
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataOnlineResource** | array | Online location where the metadata is available. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; linkage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6-0-0) |
| name |string | Name of the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; name</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; protocol</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6-0-3) |
| function |string | Function performed by the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; function &gt; CI_OnlineFunctionCode [codelist]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-6-0-4) |

## metadataRepository
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadataRepository** | array | Identifies repositories for distribution of the resource metadata. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3) |
| repository |string | Identifier for the metadata repository to which the metadata record is to be pushed. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-0) |
| metadataStandard |string | Indicates in what format the metadata record should be delivered to the repository. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-1) |
| [citation](#citation) |object | Citation for the repository. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=3-0-2) |

## metadata
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **metadata** | object | The main body of the metadata record. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata</li></ul></li><li>FGDC CSDGM<ul><li>metadata</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2) |
| [metadataInfo](#metadatainfo) |object | General information about the metadata record. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0) |
| [resourceInfo](#resourceinfo) |object | Information about the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Metadata &gt; identificationInfo &gt; MD_DataIdentification</li></ul></li><li>FGDC CSDGM<ul><li>idinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| [resourceLineage](#resourcelineage) |array | Information on the history of the resource. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| [resourceDistribution](#resourcedistribution) |array | Information about the distributor of and options for obtaining the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Metadata &gt; distribution &gt; MD_Distribution</li></ul></li><li>FGDC CSDGM<ul><li>distinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| [associatedResource](#associatedresource) |array | Other resources which are directly related to the subject resource such as parent, child, or sibling datasets or projects. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4) |
| [additionalDocumentation](#additionaldocumentation) |array | Other documents related to, but not defining, the resource such as factsheets, data catalog pages, award documents, proposals, and informational websites. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; aggregationInfo &gt; MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5) |
| [funding](#funding) |array | Information about funding for the resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-6) |

## observer
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **observer** | array | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; obs &gt; CI_ResponsibleParty</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-3) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-3-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-3-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-3-0-2) |

## offlineOption
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **offlineOption** | array | Information about obtaining the resource through off-line procedure. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; offline &gt; MD_Medium</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3) |
| [mediumSpecification](#mediumspecification) |object | Name of the formaton which the resource may be stored | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Medium &gt; name [MD_MediumNameCode]</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn &gt; offmedia</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-0) |
| density |number | Density at which the data are recorded. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-1) |
| units |string | Units of measure for the recording density. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-2) |
| numberOfVolumes |integer | The number of items identified in the media resource. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-3) |
| mediumFormat |array | Method used by the resource provider to write to the medium, such as: tar, iso9660, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Medium &gt; mediumFormat [MD_MediumFormatCode]</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn &gt; recfmt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-4) |
| note |string | Description of other limitations or requirements for using the medium. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Medium &gt; mediumNote</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn &gt; compat</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-5) |
| [identifier](#identifier) |object | Unique identifier for the medium. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3-0-6) |

## onlineOption
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **onlineOption** | array | Information about obtaining the resource on-line. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; online &gt; CI_OnlineResource</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; onlinopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-2) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; linkage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-2-0-0) |
| name |string | Name of the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; name</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-2-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; protocol</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-2-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-2-0-3) |
| function |string | Function performed by the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; function &gt; CI_OnlineFunctionCode [codelist]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-2-0-4) |

## onlineResource
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **onlineResource** | array | On-line information related to the citation. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-9) |
| uri |string | Location (address) for on-line access using a Uniform Resource Identifier, usually in the form of a Uniform Resource Locator (URL). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; linkage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-9-0-0) |
| name |string | Name of the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; name</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-9-0-1) |
| protocol |string | The connection protocol to be used such as: ftp, http, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; protocol</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-9-0-2) |
| description |string | Detailed text description of what the online resource is/does. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-9-0-3) |
| function |string | Function performed by the online resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_OnlineResource &gt; function &gt; CI_OnlineFunctionCode [codelist]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-9-0-4) |

## orderProcess
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **orderProcess** | array | Provides information about how the resource may be obtained and related instructions and fee information. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributionOrderProcess</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-1) |
| fees |string | Fees and terms for retrieving the resource, including monetary units. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; fees</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; fees</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-1-0-0) |
| plannedAvailability |string | Date and time when the resource will be available. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; plannedAvailabilityDateTime</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-1-0-1) |
| orderingInstructions |string | General instructions, terms and services provided by the distributor. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; orderingInstructions</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; onlinopt &gt; accinstr</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-1-0-2) |
| turnaround |string | Typical turnaround time for the filling of an order. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_StandardOrderProcess &gt; turnaround</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; turnarnd</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-1-0-3) |

## otherMetadataLocale
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **otherMetadataLocale** | array | Additional localised language(s) and characterset(s) used within the metadata record. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3) |
| language |string | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3-0-0) |
| characterSet |string | Full name of the character encoding standard used by the resource(see http://www.iana.org/assignments/character-sets/character-sets.xhtml). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3-0-1) |
| country |string | Designation of the specific country of the locale language(ISO 3166-1). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-3-0-2) |

## otherResourceLocale
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **otherResourceLocale** | array | Alternate localised language(s) and characterset(s) used within the resource. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24) |
| language |string | Language(s) used within the resource. Should be a valid ISO 639-3 code. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; language</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-0) |
| characterSet |string | Full name of the character encoding standard used by the resource(see http://www.iana.org/assignments/character-sets/character-sets.xhtml). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-1) |
| country |string | Designation of the specific country of the locale language(ISO 3166-1). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; characterSet [MD_CharacterSetCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24-0-2) |

## parameterCitation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **parameterCitation** | array | Reference providing description of the parameters. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-5-0-10) |

## parentMetadata
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **parentMetadata** | object | Identifier of the metadata to which this metadata is a subset (child). |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; parentIdentifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-0-1-10) |

## party
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **party** | array | Identifies all the contacts associated with the role. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-2) |
| contactId |string | Identifier matching a contactId in the main contact array. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-2-0-0) |
| organizationMembers |array | Identifies individuals that have an association with an organization contact. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-2-0-1) |

## phone
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **phone** | array | Supplemental instructions on how or when to contact the individual or organization. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Contact &gt; contactInstructions</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntinst</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-6) |
| phoneName |string | Descriptive name of the phone number. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-6-0-0) |
| phoneNumber |string | Telephone number. Recommended format is to use 'x' or 'ext' to denote extensions. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Telephone &gt; voice &#124; facsimile</li></ul></li><li>FGDC CSDGM<ul><li>cntinfo &gt; cntvoice</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-6-0-1) |
| service |array | Type(s) of phone number, e.g. voice, sms. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=1-0-6-0-2) |

## pointOfContact
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **pointOfContact** | array | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; pointOfContact</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9-0-2) |

## processStep
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **processStep** | array | A brief statement describing an individual, non-trivial process or methodology step taken in development of the resource data within the data quality scope. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Lineage &gt; processStep &gt; LI_ProcessStep</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |
| stepId |string | Serial identifier used to order the sequence of steps used. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep @ id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-0) |
| description |string | Description of the process or methodology step. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; description</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; procdesc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-1) |
| rationale |string | Requirement or purpose for the process or methodology step. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; rationale</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-2) |
| [timePeriod](#timeperiod) |object | Date, datetime, or period at which the process or methodology step occurred. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; dateTime</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; procdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-3) |
| [processor](#processor) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; processor &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; proccont &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-4) |
| [reference](#reference) |array | Citation for process step documentation. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-5) |
| [scope](#scope) |object | Type of resource and/or extent to which the process information. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3-0-6) |

## processingLevelCode
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **processingLevelCode** | object | Code that identifies the level of radiometric and geometric processing that has been applied. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_ImageDescription &gt; processingLevelCode &gt; RS_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16-0-2-4) |

## processor
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **processor** | array | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; processor &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; proccont &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-4) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-4-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-4-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-4-0-2) |

## properties
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **properties** | ambiguous | JSON object containing information about a feature or collection. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-2-0-3-1-4-4-0-1-0-1-0-3-0-1-0-1-2-2) |

## referenceSystemIdentifier
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **referenceSystemIdentifier** | object | The reference system identifier or definition. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-2-0-3-1) |
| identifier |string | A name that is used to identify the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-2-0-3-1-0) |
| namespace |string | A string which unambiguously defines the namespace for the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; codeSpace</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-2-0-3-1-1) |
| version |string | The version of the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>RS_Identifier &gt; version</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-2-0-3-1-2) |
| description |string | A natural language description of the meaning of the identifier value. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-2-0-3-1-3) |
| [authority](#authority) |object | Citation for the authority issuing the identifier. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier &gt; authority &gt; CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-2-0-3-1-4) |

## referenceSystem
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **referenceSystem** | object | Spatial reference system used by the source. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-4) |
| referenceSystemType |string | Type of reference system used. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-4-0) |
| [referenceSystemIdentifier](#referencesystemidentifier) |object | The reference system identifier or definition. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-4-1) |

## reference
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **reference** | array | Citation for the limitation or constraint |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-10) |

## releasability
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **releasability** | object | Information concerning the parties to who the resource can or cannot be released. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5) |
| [addressee](#addressee) |array | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5-0) |
| statement |string | The release statement. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5-1) |
| disseminationConstraint |array | Factor in determining releasability | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-5-2) |

## repository
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **repository** | object | Information about the curator or contact person and/or agency responsible for the specimens. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Vouchers &gt; reposit &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers &gt; reposit</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6-0-1) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6-0-1-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6-0-1-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6-0-1-2) |

## resolution
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resolution** | object | The degree of detail in the grid. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation &gt; axisDimensionProperties &gt; MD_Dimension &gt; resolution</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-2) |
| type |enum: distance, length, angle, measure, scale | The type of measurement. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-2-0) |
| value |number | The number of units in the measurement. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-2-1) |
| unitOfMeasure |string | The type of units to associated with the value. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0-0-1-0-2-2) |

## resourceCitation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceCitation** | object | Citation for the associated resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_AggregateInformation &gt; aggregateDataSetName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; crossref &gt; citeinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-4-0-3-10) |

## resourceDistribution
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceDistribution** | array | Information about the distributor of and options for obtaining the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Metadata &gt; distribution &gt; MD_Distribution</li></ul></li><li>FGDC CSDGM<ul><li>distinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3) |
| description |string | A description of a set of distribution options. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-0) |
| [distributor](#distributor) |array | Information about the distributor of and options for obtaining the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution</li></ul></li><li>FGDC CSDGM<ul><li>distinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1) |

## resourceFormat
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceFormat** | array | Provides a description of the format of the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceFormat &gt; MD_Format</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| [formatSpecification](#formatspecification) |object | Citation of the specification for the format. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Format &gt; name</li><li>MD_Format &gt; version</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtinfo &gt; formname</li><li>idinfo &gt; citation &gt; citeinfo &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-0) |
| amendmentNumber |string | Amendment number of the format version. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-1) |
| compressionMethod |string | Recommendations of algorithms or processes that can be applied to read or expand resources to which compression techniques have been applied. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19-0-2) |

## resourceInfo
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceInfo** | object | Information about the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Metadata &gt; identificationInfo &gt; MD_DataIdentification</li></ul></li><li>FGDC CSDGM<ul><li>idinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1) |
| [resourceType](#resourcetype) |array | Identifies the type of resource, such as: a dataset, study, publication, etc. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; hierarchyLevel [MD_ScopeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-0) |
| [citation](#citation) |object | Citation for the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; citation &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-1) |
| abstract |string | Brief narrative summary of the content of the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; abstract</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; descript &gt; abstract</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-2) |
| shortAbstract |string | A short description of the resource. Max of 300 characters. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-3) |
| purpose |string | A summary of intentions for which the resource was created. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; purpose</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; descript &gt; purpose</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-4) |
| [timePeriod](#timeperiod) |object | Time period for the resource, e.g. project start and end date(s). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; temporalElement &gt; EX_TemporalExtent &gt; extent &gt; TimePeriod</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-5) |
| credit |array | A narrative identification of additional resources credited for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; credit</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; datacred</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-6) |
| status |array | Status of the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; status [MD_ProgressCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; status &gt; progress</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-7) |
| <span class="md-deprecated">topicCategory</span> |array | **This property is deprecated in favor of using a keyword entry with a type of "isoTopicCategory".**

General theme keyword of the resource, such as: oceans, biota atmosphere, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; topicCategory</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-8) |
| [pointOfContact](#pointofcontact) |array | Identification of, and means of communication with, person(s) and organizations that may be contacted for acquiring knowledge about or acquisition of the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; pointOfContact</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-9) |
| [spatialReferenceSystem](#spatialreferencesystem) |array | Geospatial referencing system used in the the data resource. The reference can be provided by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Metadata &gt; referenceSystemInfo &gt; MD_ReferenceSystem &gt; referenceSystemIdentifier &gt; RS_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-10) |
| spatialRepresentationType |array | Format of the resource geographic extent, such as: vector, grid, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdenification &gt; spatialRepresentationType [MD_SpatialRepresentationTypeCode]</li></ul></li><li>FGDC CSDGM<ul><li>spdoinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-11) |
| [spatialRepresentation](#spatialrepresentation) |array | Method used to spatially represent geographic information. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12) |
| [spatialResolution](#spatialresolution) |array | Information about the scale of the geographic extent. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdenification &gt; spatialResolution &gt; MD_Resolution</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13) |
| [temporalResolution](#temporalresolution) |array | Information about the termporal period of the resource. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14) |
| [extent](#extent) |array | Information about the geographic, vertical, and temporal extent of the resource. A resource may have multiple extents. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; extent &gt; EX_Extent</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-15) |
| [coverageDescription](#coveragedescription) |array | Details about the content of a raster(grid) resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; contentInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-16) |
| [taxonomy](#taxonomy) |object | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; taxonomy</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| [graphicOverview](#graphicoverview) |array | Provides a path or link to images, maps, flow charts, models, etc. that illustrate the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; graphicOverview &gt; MD_BrowseGraphic</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-18) |
| [resourceFormat](#resourceformat) |array | Provides a description of the format of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceFormat &gt; MD_Format</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-19) |
| [keyword](#keyword) |array | Provides category keywords, their type, and reference source. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; descriptiveKeywords &gt; MD_Keywords</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; keywords</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20) |
| [resourceUsage](#resourceusage) |array | Description of ways in which the resource is currently or has been used. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceSpecificUsage &gt; MD_Usage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| [constraint](#constraint) |array | Provides information about constraints to the use of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-22) |
| [defaultResourceLocale](#defaultresourcelocale) |object | Localised language(s) and characterset(s) used within the resource. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-23) |
| [otherResourceLocale](#otherresourcelocale) |array | Alternate localised language(s) and characterset(s) used within the resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-24) |
| [resourceMaintenance](#resourcemaintenance) |array | Information about the maintenance of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| environmentDescription |string | Description of the dataset in the producer's processing environment, including items such as the software, the computer, the computer operating system, file name, and the dataset size. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; environmentDescription</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; native</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-26) |
| supplementalInfo |string | Any other descriptive information about the dataset. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; supplementalInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-27) |

## resourceLineage
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceLineage** | array | Information on the history of the resource. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2) |
| statement |string | A general statement of the actions taken to verify, transform, repair, and integrate the data within the data quality scope. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Lineage &gt; statement</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-0) |
| [scope](#scope) |object | Type of resource and/or extent to which the lineage information applies. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-1) |
| [citation](#citation) |array | Citation to a reference that describes the lineage. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-2) |
| [processStep](#processstep) |array | A brief statement describing an individual, non-trivial process or methodology step taken in development of the resource data within the data quality scope. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Lineage &gt; processStep &gt; LI_ProcessStep</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-3) |
| [source](#source) |array | Information about the source data used in creating the data identified by the data quality scope. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Lineage &gt; source &gt; LI_Source</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; srcinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4) |

## resourceMaintenance
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceMaintenance** | array | Information about the maintenance of the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceMaintenance &gt; MD_MaintenanceInformation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25) |
| frequency |string | Describes the frequency of additions and updates made to a resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceAndUpdateFrequency [MD_MaintenanceFrequencyCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-0) |
| [date](#date) |array | Date related to resource maintenance. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-1) |
| [scope](#scope) |array | Type of resource to which the maintenance information applies. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-2) |
| note |array | Notes regarding the maintenance of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; maintenanceNote</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-3) |
| [contact](#contact) |array | Contact information for the maintainer of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_MaintenanceInformation &gt; contact &gt; CI_Contact</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; metc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-4) |

## resourceType
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceType** | array | Identifies the type of resource, such as: userGuide, website, report, etc. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>[MD_ScopeCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-0) |
| type |string | The type of resource(or component of a resource) being described. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-0-0-0) |
| name |string | The name of the resource component. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-5-0-0-0-1) |

## resourceUsage
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **resourceUsage** | array | Description of ways in which the resource is currently or has been used. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; resourceSpecificUsage &gt; MD_Usage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21) |
| specificUsage |string | A brief description about how the resource is being used. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Usage &gt; specific usage</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-0) |
| [temporalExtent](#temporalextent) |array | Date and time of the first use or range of uses of the resource and/or resource series. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-1) |
| userDeterminedLimitation |string | A brief description of applications, determined by the user, for which the resource is not suitable. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Usage &gt; userDeterminedLimitations</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-2) |
| limitationResponse |array | Response to the user-determined limitations. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-3) |
| [documentedIssue](#documentedissue) |object | Citation of a description of known issues associated with the resource along with proposed solutions if available. | false | <ul class="md-translation"><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo</li></ul></li><li>ISO 19115-2<ul><li>CI_Citation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-4) |
| [additionalDocumentation](#additionaldocumentation) |array | Publications that describe usage of data. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-5) |
| [userContactInfo](#usercontactinfo) |array | Identification of the persons and/or organizations that are using the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Usage &gt; userContactInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-6) |

## responsibleParty
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **responsibleParty** | array | Entity responsible for the resource constraint |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-2) |

## responsibleParty
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **responsibleParty** | object | Name, address, country, and telecommunications address of person or organization having primary responsibility for the intellectual content of this dictionary. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-2) |

## roleExtent
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **roleExtent** | array | The area or period of time for which the role is valid. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1) |
| description |string | Description of the extent. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1-0-0) |
| [geographicExtent](#geographicextent) |array | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1-0-1) |
| [verticalExtent](#verticalextent) |array | An array of objects each describing a vertical boundary comprising all or a portion of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; verticalElement &gt; EX_VerticalExtent </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1-0-2) |
| [temporalExtent](#temporalextent) |array | An array of objects each describing a temporal boundary comprising all or a portion of the resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1-0-3) |

## schema
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **schema** | object | Identifies the version of the JSON schema standard that applies to the metadata. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0) |
| name |string | Schema identifier, i.e. the name of the schema standard. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-0) |
| version |string | Specific version number of the schema standard. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=0-1) |

## scopeDescription
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **scopeDescription** | array | Detailed description/listing of the items specified by the scope. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-1) |
| dataset |string | Dataset to which the information applies. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-1-0-0) |
| attributes |string | Instances of attribute types to which the information is applied. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-1-0-1) |
| features |string | Instances of feature types to which the information is applied. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-1-0-2) |
| other |string | Class of information that does not fall into the other categories to which the information applies. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-1-0-3) |

## scopeExtent
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **scopeExtent** | array | Information about the horizontal, vertical and temporal extent of the resource specified by the scope. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-2) |
| description |string | Description of the extent. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-2-0-0) |
| [geographicExtent](#geographicextent) |array | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-2-0-1) |
| [verticalExtent](#verticalextent) |array | An array of objects each describing a vertical boundary comprising all or a portion of the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; verticalElement &gt; EX_VerticalExtent </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-2-0-2) |
| [temporalExtent](#temporalextent) |array | An array of objects each describing a temporal boundary comprising all or a portion of the resource. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-2-2-0-3) |

## scope
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **scope** | array | Type of resource to which the maintenance information applies. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-2) |
| scopeCode |string | Class of information to which the resource applies. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-2-0-0) |
| [scopeDescription](#scopedescription) |array | Detailed description/listing of the items specified by the scope. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-2-0-1) |
| [scopeExtent](#scopeextent) |array | Information about the horizontal, vertical and temporal extent of the resource specified by the scope. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-25-0-2-0-2) |

## scope
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **scope** | object | temporal extent and or level of the application of the constraint restrictions. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-3-0-3-2) |
| scopeCode |string | Class of information to which the resource applies. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-3-0-3-2-0) |
| [scopeDescription](#scopedescription) |array | Detailed description/listing of the items specified by the scope. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-3-0-3-2-1) |
| [scopeExtent](#scopeextent) |array | Information about the horizontal, vertical and temporal extent of the resource specified by the scope. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-3-0-3-2-2) |

## security
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **security** | object | Handling restrictions imposed on the resource or metadata for national security or similar security concerns. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_SecurityConstraints</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-8) |
| classification |string | Name of the handling restrictions on the resource or metadata. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; classification [MD_ClassificationCode]</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-8-0) |
| userNote |string | Explanation of the application of the legal constraints or other restrictions and legal prerequisites for obtaining and using the resource or metadata. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; userNote</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-8-1) |
| classificationSystem |string | Name of the classification system associated with a security constraint. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; classificationSystem</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-8-2) |
| handlingDescription |string | Additional description regarding the security handling of the resource or metadata. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_SecurityConstraints &gt; handlingDescription</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-8-3) |

## series
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **series** | object | Information about the series, or aggregate resource, to which a resource belongs. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-7) |
| seriesName |string | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-7-0) |
| seriesIssue |string | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-7-1) |
| issuePage |string | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-4-0-7-2) |

## sourceCitation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **sourceCitation** | object | A citation providing information about the source dataset, including an online resource or other access instructions. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Source &gt; sourceCitation &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; srcinfo &gt; srccite &gt; citeinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1-10) |

## sourceProcessStep
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **sourceProcessStep** | array | A description of a non-trivial event or transformation taken to prepare the source data for use in creating the data identified by the data quality scope. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Source &gt; sourceStep &gt; LI_ProcessStep</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5) |
| stepId |string | Serial identifier used to order the sequence of steps used. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep @ id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-0) |
| description |string | Description of the process or methodology step. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; description</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; procdesc</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-1) |
| rationale |string | Requirement or purpose for the process or methodology step. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; rationale</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-2) |
| [timePeriod](#timeperiod) |object | Date, datetime, or period at which the process or methodology step occurred. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; dateTime</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; procdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-3) |
| [processor](#processor) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the process or methodology step. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_ProcessStep &gt; processor &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; procstep &gt; proccont &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-4) |
| [reference](#reference) |array | Citation for process step documentation. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-5) |
| [scope](#scope) |object | Type of resource and/or extent to which the process information. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5-0-6) |

## source
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **source** | array | Information about the source data used in creating the data identified by the data quality scope. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Lineage &gt; source &gt; LI_Source</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; srcinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4) |
| description |string | A brief description about the source dataset used in creating the data identified by the data quality scope. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Source &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-0) |
| [sourceCitation](#sourcecitation) |object | A citation providing information about the source dataset, including an online resource or other access instructions. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Source &gt; sourceCitation &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>dataqual &gt; lineage &gt; srcinfo &gt; srccite &gt; citeinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-1) |
| [metadataCitation](#metadatacitation) |array | Citation providing information about the metadata for the source. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-2) |
| [spatialResolution](#spatialresolution) |ambiguous | The number below the line in a vulgar fraction | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3) |
| [referenceSystem](#referencesystem) |object | Spatial reference system used by the source. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-4) |
| [sourceProcessStep](#sourceprocessstep) |array | A description of a non-trivial event or transformation taken to prepare the source data for use in creating the data identified by the data quality scope. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>LI_Source &gt; sourceStep &gt; LI_ProcessStep</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-5) |
| [scope](#scope) |object | Type of resource and/or extent to which the process information. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-6) |

## spatialReferenceSystem
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **spatialReferenceSystem** | array | Geospatial referencing system used in the the data resource. The reference can be provided by an EPSG number, a named reference, or providing the parameters in a well known text (WKT) format. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Metadata &gt; referenceSystemInfo &gt; MD_ReferenceSystem &gt; referenceSystemIdentifier &gt; RS_Identifier &gt; code</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-10) |
| referenceSystemType |string | Type of reference system used. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-10-0-0) |
| [referenceSystemIdentifier](#referencesystemidentifier) |object | The reference system identifier or definition. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-10-0-1) |

## spatialRepresentation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **spatialRepresentation** | array | Method used to spatially represent geographic information. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12) |
| [gridRepresentation](#gridrepresentation) |object | Information about grid objects in the resource. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_GridSpatialRepresentation</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-0-0) |
| [vectorRepresentation](#vectorrepresentation) |object | Information about the vector spatial objects in the resource | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-1-0) |
| [georectifiedRepresentation](#georectifiedrepresentation) |object | A grid whose cells are regularly spaced in a geographic (i.e. lat/long) or map coordinate system defined in the SpatialReferencing System (SRS) so that any cell in the grid can be geolocated given its grid coordinates and the grid origin, cell spacing, and orientation. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-2-0) |
| [georeferenceableRepresentation](#georeferenceablerepresentation) |object | Grid with cells irregularly spaced in any given geographic/map projection coordinate system, whose individual cells can be geolocated using geolocation information supplied with the data but cannot be geolocated from the grid properties alone. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-3-0) |

## spatialResolution
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **spatialResolution** | ambiguous | The number below the line in a vulgar fraction |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3) |
| scaleFactor |number | Scale of geographic extent expressed in a hardcopy map scale fraction (denominator). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Resolution &gt; equivalentScale &gt; MD_RepresentativeFraction &gt; denominator &gt; Integer</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3-0-0-0) |
| [measure](#measure) |object | Scale of geographic extent expressed in ground distance parameters or angle. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3-0-1-0) |
| levelOfDetail |string | A brief textual description of the spatial resolution of the resource | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-2-0-4-0-3-0-2-0) |

## spatialResolution
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **spatialResolution** | array | Information about the scale of the geographic extent. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdenification &gt; spatialResolution &gt; MD_Resolution</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13) |
| scaleFactor |number | Scale of geographic extent expressed in a hardcopy map scale fraction (denominator). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Resolution &gt; equivalentScale &gt; MD_RepresentativeFraction &gt; denominator &gt; Integer</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13-0-0-0) |
| [measure](#measure) |object | Scale of geographic extent expressed in ground distance parameters or angle. | true | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13-0-1-0) |
| levelOfDetail |string | A brief textual description of the spatial resolution of the resource | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-13-0-2-0) |

## subClassification
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **subClassification** | array | undefined |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-4-0-4-0-4-0-4-0-4-0-4-0-4-0-4) |
| taxonomicSystemId |string | The ID assigned by the taxonomic system to the taxonomicRank. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-4-0-4-0-4-0-4-0-4-0-4-0-4-0-4-0-0) |
| taxonomicRank |string | Name of the taxonomic rank for which the taxonValue is provided. Example: "Kingdom", "Division", "Phylum", "Subphylum", "SuperClass", "Class", "SubClass", "InfraClass", "Superorder", "Order", "Suborder", "Infraorder", "Superfamily", "Family", "Subfamily", "Tribe", "Subtribe", "Genus", "Species". | true | <ul class="md-translation"><li>ISO 19115-2<ul><li> MD_TaxonCl &gt; taxonrn</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; taxonrn</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-4-0-4-0-4-0-4-0-4-0-4-0-4-0-4-0-1) |
| latinName |string | Taxonomic rank value of the taxon being described. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonCl &gt; taxonrv</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; taxonrv</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-4-0-4-0-4-0-4-0-4-0-4-0-4-0-4-0-2) |
| commonName |array | Specification of applicable common names. These common names may be general descriptions of a group of organisms if appropriate (e.g. insects, vertebrate, grasses, waterfowl, vascular plants, etc.). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonCl &gt; common</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; common</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-4-0-4-0-4-0-4-0-4-0-4-0-4-0-4-0-3) |
| [subClassification](#subclassification) |array | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-4-0-4-0-4-0-4-0-4-0-4-0-4-0-4-0-4) |

## taxonomicClassification
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **taxonomicClassification** | object | Information about the range of taxa addressed in the data set or collection. NOTE It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxonCl &gt; MD_TaxonCl</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7) |
| taxonomicSystemId |string | The ID assigned by the taxonomic system to the taxonomicRank. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-0) |
| taxonomicRank |string | Name of the taxonomic rank for which the taxonValue is provided. Example: "Kingdom", "Division", "Phylum", "Subphylum", "SuperClass", "Class", "SubClass", "InfraClass", "Superorder", "Order", "Suborder", "Infraorder", "Superfamily", "Family", "Subfamily", "Tribe", "Subtribe", "Genus", "Species". | true | <ul class="md-translation"><li>ISO 19115-2<ul><li> MD_TaxonCl &gt; taxonrn</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; taxonrn</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-1) |
| latinName |string | Taxonomic rank value of the taxon being described. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonCl &gt; taxonrv</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; taxonrv</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-2) |
| commonName |array | Specification of applicable common names. These common names may be general descriptions of a group of organisms if appropriate (e.g. insects, vertebrate, grasses, waterfowl, vascular plants, etc.). | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonCl &gt; common</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl &gt; common</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-3) |
| [subClassification](#subclassification) |array | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7-4) |

## taxonomicSystem
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **taxonomicSystem** | array | Information about the taxonomic classification system used. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; classSys</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; classsys</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0) |
| [citation](#citation) |object | Information about the classification system or authority used. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; classSys &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; classsys</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-0-0) |
| modifications |string | Description of any modifications or exceptions made to the classification system or authority used. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0-0-1) |

## taxonomy
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **taxonomy** | object | Information on the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DataIdentification &gt; taxonomy</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17) |
| [taxonomicSystem](#taxonomicsystem) |array | Information about the taxonomic classification system used. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; classSys</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; classsys</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-0) |
| generalScope |string | Description of the range of taxa addressed in the data set or collection. For example, "all vascular plants were identified to family or species, mosses and lichens were identified as moss or lichen". | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxongen</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-1) |
| [identificationReference](#identificationreference) |array | Information on any non-authoritative materials (e.g. field guides) useful for reconstructing the actual process. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-2) |
| [observer](#observer) |array | Information about the individual(s) responsible for the identification(s) of the specimens or sightings. etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; obs &gt; CI_ResponsibleParty</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-3) |
| identificationProcedure |string | Description of the methods used for taxonomic identification. Could include specimen processing, comparison with museum materials, keys, and key characters, chemical or genetic analyses, etc. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxonpro</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; taxonpro</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-4) |
| identificationCompleteness |string | Information concerning the proportions and treatment of unidentified materials (i.e. materials sent to experts, and not yet determined); estimates of the importance, and identities of misidentifications, uncertain determinations, synonyms or other incorrect usages; taxa not well treated or requiring further work; and expertise of field workers. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-5) |
| [voucher](#voucher) |array | Information on the types of specimen, the repository, and the individuals who identified the vouchers. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; voucher &gt; MD_Vouchers</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6) |
| [taxonomicClassification](#taxonomicclassification) |object | Information about the range of taxa addressed in the data set or collection. NOTE It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; taxonCl &gt; MD_TaxonCl</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxoncl</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-7) |

## temporalExtent
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **temporalExtent** | array | An array of objects each describing a temporal boundary comprising all or a portion of the resource. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1-0-3) |

## temporalResolution
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **temporalResolution** | array | Information about the termporal period of the resource. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14) |
| years |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-0) |
| months |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-1) |
| days |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-2) |
| hours |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-3) |
| minutes |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-4) |
| seconds |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-14-0-5) |

## thesaurus
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **thesaurus** | object | Name of the formally registered thesaurus or a similar authoritative source of keywords. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Keywords &gt; thesaurusName &gt; CI_Citation</li></ul></li><li>FGDC CSDGM<ul><li>idinfo&gt;keywords&gt;theme&gt;themekt</li><li>idinfo&gt;keywords&gt;place&gt;placekt</li><li>idinfo&gt;keywords&gt;temporal&gt;tempkt</li><li>idinfo&gt;keywords&gt;stratum&gt;stratkt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2) |
| title |string | Name by which the cited resource is known. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; title</li><li>FC_FeatureCatalogue &gt; name</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; citeinfo &gt; title</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-0) |
| alternateTitle |array | Alias by which the cited resource is known. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; alternateTitle</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-1) |
| [date](#date) |array | Date referenced to the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; date &gt; CI_Date</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-2) |
| edition |string | Version identifier for the resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; edition</li><li>FC_FeatureCatalogue &gt; versionNumber</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; edition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-3) |
| [responsibleParty](#responsibleparty) |array | Identification of, and means of communication with, person(s) and organization(s) associated with the cited resource. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty</li><li>FC_FeatureCatalogue &gt; producer &gt; CI_ResponisbleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; ptcontac &gt; cntinfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-4) |
| presentationForm |array | The form that the resource is presented, such as: digital map, digital document, etc. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; presentationForm [CI_PresentationFormCode]</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; citation &gt; geoform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-5) |
| [identifier](#identifier) |array | Identifier for the resource in the context of the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-6) |
| [series](#series) |object | Information about the series, or aggregate resource, to which a resource belongs. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-7) |
| otherCitationDetails |array | Other information required to complete the citation that is not recorded elsewhere. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-8) |
| [onlineResource](#onlineresource) |array | On-line information related to the citation. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>CI_Citation &gt; citedResponsibleParty &gt; CI_ResponsibleParty &gt; contact &gt; CI_Contact &gt; onlineResource &gt; CI_OnlineResource</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-9) |
| [graphic](#graphic) |array | Online graphic associated with the citation | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-20-0-2-10) |

## timeInstant
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **timeInstant** | object | Represents an identifiable position in time. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-0-0) |
| id |string | A unique identifier for the timeInstant. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-0-0-0) |
| [identifier](#identifier) |object | Identifier assigned to the timeInstant. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-0-0-1) |
| description |string | A brief description providing relevant information about the date and time. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant &gt; description</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-0-0-2) |
| instantName |array | Name of the timeInstant | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-0-0-3) |
| dateTime |string | An ISO 8601 date/timestamp. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimeInstant &gt; timePosition</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-0-0-4) |

## timeInterval
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **timeInterval** | object | Defines a length of time in specific units. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-6) |
| interval |number | The amount of time. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-6-0) |
| units |enum: year, month, day, hour, minute, second | The unit of time for the interval. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-6-1) |

## timePeriod
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **timePeriod** | object | A span of time represented by a starting date-time and an ending date-time. |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0) |
| id |string | A unique identifier for a time period. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod @id</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-0) |
| description |string | A brief description providing relevant information about the time period. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; description </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-1) |
| [identifier](#identifier) |object | Identifier for the timePeriod. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Identifier</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-2) |
| periodName |array | Names associated with the time period. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-3) |
| startDateTime |string | Starting date, or date and time. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; beginPosition </li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; timeperd &gt; rngdates &gt; begdate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-4) |
| endDateTime |string | Ending date, or date and time. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_TemporalExtent &gt; extent &gt; TimePeriod &gt; endPosition</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; timeperd &gt; rngdates &gt; enddate</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-5) |
| [timeInterval](#timeinterval) |object | Defines a length of time in specific units. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-6) |
| [duration](#duration) |object | Object for collecting information about a duration or period of time. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-4-0-1-0-3-0-0-1-0-7) |

## transferFrequency
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **transferFrequency** | object | The rate of occurrence of distribution. |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4) |
| years |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4-0) |
| months |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4-1) |
| days |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4-2) |
| hours |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4-3) |
| minutes |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4-4) |
| seconds |integer | undefined | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4-5) |

## transferOption
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **transferOption** | array | Describes method and media by which a resource is obtained from the distributor. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distributor &gt; distributorTransferOptions</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2) |
| transferSize |number | Estimated size of a unit in the specified transfer format, expressed in megabytes. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-0) |
| unitsOfDistribution |string | The tiles, layers, geographic areas, etc., in which data are available. | false | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-1) |
| [onlineOption](#onlineoption) |array | Information about obtaining the resource on-line. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; online &gt; CI_OnlineResource</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; onlinopt</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-2) |
| [offlineOption](#offlineoption) |array | Information about obtaining the resource through off-line procedure. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_DigitalTransferOptions &gt; offline &gt; MD_Medium</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform &gt; digtopt &gt; offoptn</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-3) |
| [transferFrequency](#transferfrequency) |object | The rate of occurrence of distribution. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-4) |
| [distributionFormat](#distributionformat) |array | Provides information about the format used by the distributor. | false | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Distribution &gt; distributor &gt; MD_Distributor &gt; distributorFormat &gt; MD_Format</li></ul></li><li>FGDC CSDGM<ul><li>distinfo &gt; stdorder &gt; digform</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-3-0-1-0-2-0-5) |

## userContactInfo
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **userContactInfo** | array | Identification of the persons and/or organizations that are using the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Usage &gt; userContactInfo</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-6) |
| role |string | Function performed by the contact in the current context. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MI_Metadata &gt; Contact &gt; CI_Contact &gt; role [CI_RoleCode]</li></ul></li><li>FGDC CSDGM<ul><li>metainfo &gt; cntinfo &gt; cntpos</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-6-0-0) |
| [roleExtent](#roleextent) |array | The area or period of time for which the role is valid. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-6-0-1) |
| [party](#party) |array | Identifies all the contacts associated with the role. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-21-0-6-0-2) |

## vectorObject
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **vectorObject** | array | Information about the geometric objects used in the resource |   | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-1-0-1) |
| objectType |string | Name of point or vector objects used to locate zero-, one-, two-, or three-dimensional spatial locations in the resource. | true | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-1-0-1-0-0) |
| objectCount |integer | The total number of point or vector objects occurring in the dataset. | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-1-0-1-0-1) |

## vectorRepresentation
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **vectorRepresentation** | object | Information about the vector spatial objects in the resource |   | No translation available. | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-1-0) |
| topologyLevel |string | Identifies the degree of complexity of the spatial relationships | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-1-0-0) |
| [vectorObject](#vectorobject) |array | Information about the geometric objects used in the resource | false | <ul class="md-translation"></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-12-0-0-1-0-1) |

## verticalExtent
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **verticalExtent** | array | An array of objects each describing a vertical boundary comprising all or a portion of the resource. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>EX_Extent &gt; verticalElement &gt; EX_VerticalExtent </li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=4-0-4-1-0-3-0-0-1-0-2-4-10-0-3-6-0-1-0-2) |

## voucher
| Name | Type | Description | Required | Translation | Viewer Link|
| --- | --- | --- | --- | --- | --- |
| **voucher** | array | Information on the types of specimen, the repository, and the individuals who identified the vouchers. |   | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_TaxonSys &gt; voucher &gt; MD_Vouchers</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6) |
| specimen |string | Word or phrase describing the type of specimen collected (e.g. 'herbarium specimens', 'blood samples', 'photographs', 'individuals', or 'batches'). | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Vouchers &gt; specimen</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers &gt; specimens</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6-0-0) |
| [repository](#repository) |object | Information about the curator or contact person and/or agency responsible for the specimens. | true | <ul class="md-translation"><li>ISO 19115-2<ul><li>MD_Vouchers &gt; reposit &gt; CI_ResponsibleParty</li></ul></li><li>FGDC CSDGM<ul><li>idinfo &gt; taxonomy &gt; taxonsys &gt; vouchers &gt; reposit</li></ul></li></ul> | [link](http://www.adiwg.org/mdTools/#viewer-page?v=2-1-17-6-0-1) |
