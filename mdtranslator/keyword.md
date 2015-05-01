# mdTranslator

## Architecture

### Internal Object
---
#### keyword:

The *keyword* object

````ruby
    def newKeyword
        intObj = {
            keyword: [],
            keywordType: nil,
            keyTheCitation: {}
        }
    end
````

__keyword:__ *array* (required) - an array of quoted keywords or keyword phrases

__keywordType:__ *string* - a users supplied category for the keywords provides.  e.g. 'place names', 'species', 'theme'

__keyTheCitation:__ *object* - a [citation](../mdtranslator/citation.md) object identifying the thesaurus from which the keywords were selected.
