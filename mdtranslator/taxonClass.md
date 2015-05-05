# mdTranslator

## Architecture

### Internal Object
---
#### taxonClass:

The *taxonClass* object provides a specification for the range of taxa addressed in the data set or collection. It is recommended that one provide information starting from the taxonomic rank of kingdom, to a level which reflects the data set or collection being documented. The levels of Kingdom, Division/Phylum, class, Order, Family, Genus, and Species should be included as ranks as appropriate.

````ruby
    def newTaxonClass
        intObj = {
            commonName: nil,
            taxRankName: nil,
            taxRankValue: nil
        }
    end
````

__commonName:__ *string* - specification of the common name. Common names may be general descriptions of a group of organisms if appropriate (e.g., insects, vertebrate, grasses, waterfowl, vascular plants, etc.).

__taxRankName:__ *string* (required) - name of the taxonomic rank for which the taxonValue is provided. Example: <br>
 * "Kingdom"
 * "Division"
 * "Phylum"
 * "Subphylum"
 * "SuperClass"
 * "Class"
 * "SubClass"
 * "InfraClass"
 * "Superorder"
 * "Order"
 * "Suborder"
 * "Infraorder"
 * "Superfamily"
 * "Family"
 * "Subfamily"
 * "Tribe"
 * "Subtribe"
 * "Genus"
 * "Species"
 * "Subspecies"

__taxRankValue:__ *string* (required) - the latin name or taxonomic rank value of the taxon being described
