# medium:

The *medium* object provides information about the offline media on which the resource can be obtained.

````ruby
    def newMedium
        intObj = {
            mediumName: nil,
            mediumFormat: nil,
            mediumNote: nil
        }
    end
````

__mediumName:__ *string* - the name of the medium on which the resource can be received

__mediumFormat:__ *string* - the method used by the resource provider to write to the medium, such as: tar, iso9660, etc.

__mediumNote:__ *string* - a description of other limitations or requirements for using the medium
