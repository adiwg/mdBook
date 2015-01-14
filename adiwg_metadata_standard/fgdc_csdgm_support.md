# FGDC CSDGM Support

## *Introduction*

Metadata authors and managers should understand that the Alaska Data Integration Working Group (ADIwg) metadata standard and its structural format differ from the Federal Geographic Data Committee (FGDC) metadata standard. The file type traditionally used to create and share metadata records in the FGDC Content Standards for Digital Geospatial Metadata (CSDGM) format is an eXtensible Markup Language (XML) file. Workflows for creating, editing, and validating FGDC-CSDGM records generally employ software that can read and write XML files, as well as 'validate' the XML files against a schema file that formally defines the permitted structure and content of a well-formatted FGDC-CSDGM file.

The ADIwg metadata standard is an independent metadata format that collects a different set of informational pieces (or metadata 'elements') and uses a different file format for creating and storing metadata. Rather than the XML files employed in the FGDC-CSDGM workflow, ADIwg metadata records are written in and stored as Java Script Object Notation (JSON) files. Metadata validation with ADIwg records is analagous to FGDC-CSDGM metadata validation, however a JSON schema is used instead of an XSD schema. In the same way that FGDC-CSDGM files must be compliant with the published XML standard, ADIwg JSON files must adhere to the structural specifications delineated in the ADIwg JSON schema to be valid.

While the file format, element names, and structural organization differ between ADIwg JSON metadata records and FGDC-CSDGM XML metadata records, both standards seek to capture the same fundamental information about a data product. This critical information generally includes the details about the data itself, the organization or individuals that created it, related products or resources connected to the data, access and/or use limitations, and any specific information about how to properly interpret and use the data. Although the way these different components are stored may differ between the two formats (e.g., the general description of a data resource may populated in Element 'X' in an FGDC-CSDGM XML file, while the same information may be stored in Element 'Y' in an ADIWG JSON file), almost every element in an FGDC metadata record has a corollary in the ADIwg JSON standard. To this end, it should be possible to translate or crosswalk most FGDC metadata records into the ADIwg standard. Users familiar with the FGDC standard who wish to generate new records from scratch in the ADIwg format should be able to represent the same information they would have collected in an FGDC XML file using the corresponding elements in the ADIwg JSON file.

Additionally, ADIwg metadata supports several additional pieces of information that are not necessarily present or 'supported' in the FGDC-CSDGM format. With this in mind, users should be aware that when starting with an ADIwg record or attempting to crosswalk content from an ADIwg JSON file to an FGDC-CSDGM XML, that several elements may not have a corollary in the FGDC-CSDGM format.

#### Creating an ADIwg Metadata Record

"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua."

#### Understanding 'Parallel' Elements between the ADIwg and FGDC-CSDGM Metadata Standards

"Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur."

#### Best Practices and Suggested Workflows

"Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."
