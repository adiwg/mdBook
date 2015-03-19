# resourceFormat:

The *resourceFormat* object that describes the computer language construct that specifies the representation of data objects in a record, file, message, storage device or transmission.

````ruby
    def newResourceFormat
        intObj = {
            formatName: nil,
            formatVersion: nil
        }
    end
````

__formatName:__ *string* (required) - name of the data transfer format

__formatVersion:__ *string* - version of the format, i.e. number, date, or other
