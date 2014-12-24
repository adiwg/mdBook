# Output

## Single static codelist - names only

#### Call:
From Ruby
````Ruby
codeList = ADIWG::Mdcodes.getStaticCodelist('iso_scope','json')
````

From API:
http://mdtranslator.herokuapp.com/api/codelists/iso_scope

The API will only return a JSON object.

#### Examples:
note: The lists have been truncated for purposes of examples

##### JSON return
````json
{
	"iso_scope": [
		"attribute",
		"attributeType",
		"dataDictionary",
		"website",
		"publication",
		"report",
		"awardInfo",
		"collectionSite",
		"project",
		"factSheet"
	]
}
````

##### Ruby hash return
````ruby
{"iso_scope"=>
  ["attribute",
   "attributeType",
   "dataDictionary",
   "website",
   "publication",
   "report",
   "awardInfo",
   "collectionSite",
   "project",
   "factSheet"]
}
````

## Single codelist - full detail

#### Call:
From Ruby
````Ruby
codeList = ADIWG::Mdcodes.getCodelistDetail('iso_classification','json')
````

From API:
http://mdtranslator.herokuapp.com/api/codelists/iso_classification?definitions=true

The API will only return a JSON object.

#### Example:
note: The list has been truncated for purposes of examples.  The hash example is not shown.

````json
{
	"codelistType": "staticList",
	"codelistName": "iso_classification",
	"source": "ISO",
	"sourceName": "MD_ClassificationCode",
	"extensible": true,
	"description": "name of the handling restrictions on the dataset",
	"codelist": [
		{
			"code": "001",
			"codeName": "unclassified",
			"description": "available for general disclosure"
		},
		{
			"code": "002",
			"codeName": "restricted",
			"description": "not for general disclosure"
		},
		{
			"code": "009",
			"codeName": "limitedDistribution",
			"description": "dissemination limited by designating body"
		}
	]
}
````

## All static codelists - names only

#### Call:
From Ruby
````Ruby
codeList = ADIWG::Mdcodes.getAllStaticCodelists('json')
````

From API:
http://mdtranslator.herokuapp.com/api/codelists

The API will only return a JSON object.

#### Example:
note: The list has been truncated for purposes of examples.  The hash example is not shown.

```json
{
  "iso_associationType": [
    "crossReference",
    "largerWorkCitation",
    "partOfSeamlessDatabase",
    "supplementalResource"
  ],
  "iso_characterSet": [
    "ucs2",
    "ucs4",
    "utf7",
    "utf8",
    "utf16",
    "GB2312"
  ],
  "iso_classification": [
    "unclassified",
    "restricted",
    "confidential",
    "secret",
    "topSecret",
    "sensitiveButUnclassified",
    "forOfficialUseOnly",
    "protected",
    "limitedDistribution"
  ]
}
````

## All codelists - full detail

#### Call:
From Ruby
````Ruby
codeList = ADIWG::Mdcodes.getAllCodeistsDetail('json')
````

From API:
http://mdtranslator.herokuapp.com/api/codelists?definitions=true

The API will only return a JSON object.

#### Example:
note: The list has been truncated for purposes of examples.  The hash example is not shown.

````json
{
  "iso_associationType": {
    "codelistType": "staticList",
    "codelistName": "iso_associationType",
    "source": "ISO",
    "sourceName": "DS_AssociationTypeCode",
    "extensible": true,
    "description": "justification for the correlation of two resources (datasets or projects)",
    "codelist": [
      {
        "code": "001",
        "codeName": "crossReference",
        "description": "reference from one resource (dataset or project) to another"
      },
      {
        "code": "adiwg002",
        "codeName": "supplementalResource",
        "description": "supplemental resource"
      }
    ]
  },
  "iso_characterSet": {
    "codelistType": "staticList",
    "codelistName": "iso_characterSet",
    "source": "ISO",
    "sourceName": "MD_CharacterSetCode",
    "extensible": true,
    "description": "name of the character coding standard used in the resource",
    "codelist": [
      {
        "code": "001",
        "codeName": "ucs2",
        "description": "16-bit fixed size Universal Character Set, based on ISO/IEC 10646"
      },
      {
        "code": "029",
        "codeName": "GB2312",
        "description": "simplified Chinese code set"
      }
    ]
  },
  "iso_classification": {
    "codelistType": "staticList",
    "codelistName": "iso_classification",
    "source": "ISO",
    "sourceName": "MD_ClassificationCode",
    "extensible": true,
    "description": "name of the handling restrictions on the dataset",
    "codelist": [
      {
        "code": "001",
        "codeName": "unclassified",
        "description": "available for general disclosure"
      },
      {
        "code": "009",
        "codeName": "limitedDistribution",
        "description": "dissemination limited by designating body"
      }
    ]
  }
}
````


## ISO CT_CodelistCatalogue

This format is provided as a REST endpoint [CT_CodelistCatalogue](http://mdtranslator.herokuapp.com/api/codelists?format=xml). It is intended for use as the formal ISO 'codeList=' reference in coding ISO 19115-2:2003 and 19115-1:2014 metadata codelists.  This output is only available through the API.

````xml
<gmd:role>
    <gmd:CI_RoleCode codeList="http://mdtranslator.herokuapp.com/api/codelists?format=xml#CI_RoleCode" codeListValue="author" codeSpace="011"/>
</gmd:role>

````

