# Ruby

# mdCodes Rubygem

mdCodes provides code lists in hash or JSON formats for loading of mdEditor and other metadata tools that use the ADIwg [mdJson-schemas](https://github.com/adiwg/mdJson-schemas).

Each codelists include all ISO 19115-2 and ISO 19115-1 codes plus and many codelists also carry supplemental codes added by NGDC or ADIwg. The codelists may be accessed in Ruby by installing the adiwg-mdcodes gem. Alternatively, JSON formatted codelists may be returned when using the hosted API (see next section) or  [Grunt](http://gruntjs.com/getting-started).

### Methods

#### getYamlPath
> returns the path to the 'resources' folder containing codelist files in YAML format'.

#### getAllCodelistsDetail( returnFormat )
> returns all code lists with all codelist detail
> returnFormat = \[__hash__ | json] (string)

#### getAllCodelistDetail( codeListName, returnFormat )
> returns a single codelist with all code list detail
> codeListName = name of code list to return (string)
> returnFormat = \[ __hash__ | json ] (string)

#### getAllStaticCodelists( returnFormat )
> returns all static codelists with only the codelist item names
> returnFormat = \[__hash__ | json] (string)

#### getStaticCodelist( codeListName, returnFormat )
> returns a single static codelist with only the codelist item names
> codeListName = name of code list to return (string)
> returnFormat = \[__hash__ | json] (string)


### Examples
````Ruby
require 'adiwg-mdcodes'

# get ISO role types codelist - codeNames only
codeListName = 'iso_role'
codeList = ADIWG::Mdcodes.getStaticCodelist(codeListName)

#  get all codelist with full detail
allCodeLists = ADIWG::Mdcodes.getAllCodeistsDetail

````

