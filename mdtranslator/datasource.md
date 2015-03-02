# dataSource:

The *dataSource* object provides information about the source data used in creating the data specified in the [dataScope](../mdtranslator/dataQuality.md).

````ruby
    def newDataSource
        intObj = {
            sourceDescription: nil,
            sourceCitation: {},
            sourceSteps: []
        }
    end
````

__sourceDescription:__ *string* - a brief description about the source dataset used in creating the data specificed in the scope.

__sourceCitation:__ *object* - a [citation](../mdtranslator/citation.md) object providing information about the source dataset including a link or other access instructions.

__sourceSteps:__ *array* - an array of [dataProcessingStep](../mdtranslator/dataProcessingStep.md) describing the non-trivial events and transformations to prepare the source data for use as the data specified in the scope.
