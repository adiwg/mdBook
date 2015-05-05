# mdTranslator

## Architecture

### Internal Object
---
#### taxonSystem:

The *taxonSystem* object provides information about the taxa (1 or more) included in the data set, including keywords, taxonomic system and coverage information, and taxonomic classification system.

````ruby
    def newTaxonSystem
        intObj = {
            taxClassSys: [],
            taxGeneralScope: nil,
            taxObservers: [],
            taxIdProcedures: nil,
            taxVoucher: {},
            taxClasses: []
        }
    end
````

__taxClassSys:__ *array* (required) - an array of [citation](../mdtranslator/citation.md) citation objects describing the taxonomic classification system or authority used to specify the taxonomy

__taxGeneralScope:__ *string* - a brief description of the range of taxa addressed in the data set or collection. For example, "all vascular plants were identified to family or species, mosses and lichens were identified as moss or lichen".

__taxObservers:__ *array* - an array of [responsibleParty](../mdtranslator/responsibleParty.md) objects identifying individual(s) responsible for the identification(s) of the specimens or sightings.

__taxIdProcedures:__ *string* (required) - a brief description of the methods used for taxonomic identification (e.g., specimen processing, comparison with museum materials, keys, and key characters, chemical or genetic analyses, etc).

__taxVoucher:__ *object* - an [taxonVoucher](../mdtranslator/taxonVoucher.md) object providing information on the types of specimen, the repository, and the individuals who identified the species.

__taxClasses:__ *array* (required) - an array of [taxonClass](../mdtranslator/taxonClass.md) objects providing information about the range of taxa addressed in the dataset or collection. It is recommended that metadata authors provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division, Phylum, Class, Order, Family, Genus, and Species should be included as ranks as appropriate.
