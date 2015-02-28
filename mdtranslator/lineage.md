# lineage:

The *lineage* object contains procedural (non-quantitative) data quality information about the portion of the data resource identified in the dataScope.  The procedural steps can document the steps taken to verify, transform, repair, integrate, and produce data for subsequent use.

````ruby
    def newLineage
        intObj = {
            statement: nil,
            processSteps: [],
            dataSources: []
        }
    end
````

__statement:__ *string* - a general statement of the actions taken to verify, transform, repair, and integrate the data described in the [dataScope](../mdtranslator/dataQuality.md).

__processingSteps:__ *array* - an array of [dataProcessingStep](../mdtranslator/dataProcessingStep.md) objects a contain a brief statement describing an individual, non-trivial process or methodology step taken in development of the resource data described in the [dataScope](../mdtranslator/dataQuality.md).

__dataSources:__ *array* - an array of [dataSource](../mdtranslator/dataSource.md) objects providing a reference to an existing datasets used in creating the data described in the [dataScope](../mdtranslator/dataQuality.md).
