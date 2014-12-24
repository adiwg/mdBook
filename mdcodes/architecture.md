# Architecture

## Overview

The mdCodes gem currently supports only 'static' codelists.  In the future the mdCodes
architecture may be extended to support hierarchical and/or externally hosted codelist.

## Static Codelists
Static lists are single dimensional, fixed lists with multiple items each having the
typical {code, code name, definition} paring.  Each codelist is maintained in its own
YAML file and is accessed by its name.  The codelist is returned as either a JSON object
or a Ruby hash depending on the format requested.



