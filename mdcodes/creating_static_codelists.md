# Creating Static Codelists

## Steps

1. Create YAML file of your codelist in mdCodes format.
2. Place the YAML file in the mdCodes > resources directory.
3. Rebuild and install the mdCodes Rubygem.

## mdCodes YAML file format

### Template:

#### Items in static codelist:
* **codelistType**
   String (Required): for static codelists this must be "staticList"
* **codelistName**
   String (Required): name you assign to the codelist.  This will also be the file name of the YAMLfile (e.g. codelistname.yml).
* **source**
   String: name of the primary organization to established the codelist codes, codenames, and definitions.
* **sourceName**
   String: name the source organization has assigned to the codelist.
* **extensible**
   Boolean: can the codelist be extended? i.e. can new items be added to the codelist or items be removed?
* **description**
   String: definition for the codelist.
* **codelist**
   Array (Required): codelist items
  * **code**
     String (Required): code or value for the item.  Usually hidden from display.
  * **codeName**
     String (Required): name for the item.  Usually displayed to the user through dropdown or other selection control.
  * **description**
     String (Required): definition of the item


````yaml
---
# comments

codelistType: "staticList"
codelistName: <<codelist name>>
source: <<organization that manages the codelist>>
sourceName: <<name the source has given to the codelist>>
extensible: <<can the code list be extended? true|false>>
description: <<description>>
codelist:
  - {code: <<id>>, codeName: <<name>>, description: <<description>>}
  - {code: <<id>>, codeName: <<name>>, description: <<description>>}
  ...
````

### Example:
````yaml
---
# mdJson codelists
# base codelist for ISO 19115-2, 19115-1
# extended for ADIwg

codelistType: "staticList"
codelistName: "iso_associationType"
source: "ISO"
sourceName: "DS_AssociationTypeCode"
extensible: true
description: "justification for the correlation of two resources (datasets or projects)"
codelist:
  - {code: "001", codeName: crossReference, description: "reference from one resource (dataset or project) to another"}
  - {code: "002", codeName: largerWorkCitation, description: "reference to a master resource (dataset or project) of which this one is a part"}
````


