# taxonVoucher:

The *taxonVoucher* object providing information on the types of specimen, the repository, and the individuals who identified the vouchers.

````ruby
    def newTaxonVoucher
        intObj = {
            specimen: nil,
            repository: {}
        }
    end
````

__specimen:__ *string* (required) - a word or phrase describing the type of specimen collected.  e.g. 'herbarium specimens', 'blood samples', 'photographs', 'individuals'

__repository:__ *object* (required) - a [responsibleParty](../mdtranslator/responsibleParty.md) object
