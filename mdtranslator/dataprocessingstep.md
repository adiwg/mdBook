# dataProcessingStep:

The *dataProcessingStep* object provides a brief statement about a discrete non-trivial event or transformation in the life of a dataset including processes used to manage the quality of the data.

````ruby
    def newDataProcessStep
        intObj = {
            stepId: nil,
            stepDescription: nil,
            stepRationale: nil,
            stepDateTime: {},
            stepProcessors: []
        }
    end
````

__stepId:__ *string* - a user provided ID for the step.

__stepDescription:__ *string* (required) - description of the event or transformation including any related parameters or tolerances.

__stepRationale:__ *string* - requirement or purpose for the process step.

__stepDateTime:__ *dateTime* - date and time or date at which the process or methodology step occurred.

__stepProcessor:__ *array* - an array of [responsibleParty](../mdtranslator/responsibleParty.md) objects identifying persons and/or organizations and their roles associated with the process step.
