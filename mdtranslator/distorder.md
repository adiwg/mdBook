# distOrder:

The *distOrder* object provides information about how the resource may be obtained including related instructions and fee information.

````ruby
    def newDistOrder
        intObj = {
            fees: nil,
            plannedDateTime: {},
            orderInstructions: nil,
            turnaround: nil
        }
    end
````

__fees:__ *string* - fees and terms for retrieving the resource, including monetary units

__plannedDateTime:__ *dateTime* - a [dateTime](../mdtranslator/dateTime.md) object providing the date and time after which the resource will be available

__orderInstructions:__ *string* - general instrucions, terms, and servicesprovided by the distributor

__turnaround:__ *string* - typical turnaround time for the filling of an order
