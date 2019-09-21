# mdJSON Schemas
[![Build Status](https://travis-ci.org/adiwg/mdJson-schemas.svg?branch=master)](https://travis-ci.org/adiwg/mdJson-schemas)
[![Gem Version](https://badge.fury.io/rb/adiwg-mdjson_schemas.svg)](http://badge.fury.io/rb/adiwg-mdjson_schemas)
[![npm version](https://badge.fury.io/js/mdjson-schemas.svg)](https://badge.fury.io/js/mdjson-schemas)

![mdJSON Schemas](/assets/logos/mdJSONSchemas_logo.png)

ADIwg metadata can be translated and exported as ISO 19115-2/19110 or 19115-1 records in XML documents that conform to ISO 19139 or 19115-3, the international standard that defines the structure and syntax required for the exchange of ISO 19115 metadata. XML is a widely used World Wide Web Consortium (WC3) standard for sharing and exchanging self-describing, machine-readable content. XML documents can be validated against XML Schema Documents to determine whether the XML document structurally and syntactically conforms with the requirements defined in the schema. This ability to verify the conformance of content documents with schema documents makes XML an appealing choice for metadata storage and exchange across many data centers and systems.

However, despite its strengths, XML is a verbose, cumbersome medium for data processing or storage. To address these inefficiencies, the ADIwg technical group chose to create, store, and process ADIwg metadata in JSON. Compared to XML, JSON provides more concise, compact, and human-readable code that is easier for developers to ingest and modify. The development of JSON schemas allows for the specification and validation of JSON file structure, syntax, and cardinality of defined data structures and elements. ADIwg metadata uses JSON schemas(mdJSON) defined by the ADIwg technical team to define repeatable, modular blocks of metadata content. These blocks describe the important aspects of data collection, processing, and preservation, and the entities responsible for the collection, processing, or modification of the data that occurs throughout the data lifecycle.

The ADIwg mdJSON schemas are briefly described in this section, and are available in their entirety on the [ADIwg GitHub page](https://github.com/adiwg/mdJson-schemas), along with examples of JSON documents conforming to each schema and populated with metadata content.

However, the [mdJSON Schema Viewer](/mdjson_schema_viewer/schema_tree.md) is the
recommended way to view the schemas.

More info about JSON schemas at [json-schema.org](http://json-schema.org/).
