# mdTranslator

## Architecture

### Internal Object
---
#### securityCon:

The *securityCon* object contains handling restrictions imposed on the resource or metadata for
national security or similar security concerns.

````ruby
    def newSecurityConstraint
        intObj = {
            classCode: nil,
            userNote: nil,
            classSystem: nil,
            handlingDesc: nil
        }
    end
````

__classCode:__ *string* (required) - name of the handling restrictions on the resource or metadata

__userNote:__ *string* - explanation of the applicability of the legal constraints or other restrictions/legal prerequisites for obtaining and using the resource or metadata

__classSystem:__ *string* - name of the classification system associated with a security constraint

__handlingDesc:__ *string* - additional description regarding the security handling of the resource or metadata
