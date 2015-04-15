# dictionaryInfo:

The *dictionaryInfo* object contains identification, descriptive, and contact information for the data dictionary.

````ruby
    def newDictionaryInfo
        intObj = {
            dictCitation: {},
            dictDescription: nil,
            dictResourceType: nil,
            dictLanguage: nil
        }
    end
````

__dictCitation:__ *object* - a [citation](../mdtranslator/citation.md) object that contains versioning and contact information for the data dictionary.

__dictDescription:__ *string* - a brief description of the data dictionary.

__dictResourceType:__ *string* - identifies the scope of the data dictionary. E.g. 'database', 'dataset', 'table'.

__dictLanguage:__ *string* - defines the language and country of origin in which the data dictionary is written (e.g., 'eng; USA', 'eng; UK', 'esp; MEX').
