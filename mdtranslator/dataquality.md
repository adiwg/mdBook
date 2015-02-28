# dataQuality:

The *dataQuality* object describes the data quality, lineage, and/or processing steps that were applied to the data resource.

````ruby
    def newDataQuality
        intObj = {
            dataScope: nil,
            dataLineage: {}
        }
    end
````

__dataScope:__ *string* - the specific scope to which the data quality information is applied, for instance a dataset, attribute, feature, series, etc.

__dataLineage:__ *object* - a [lineage](../mdtranslator/lineage.md) object that contains procedural (non-quantitative) data quality information about the portion of the data resource identified in the dataScope.
