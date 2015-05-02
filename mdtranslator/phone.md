# mdTranslator

## Architecture

### Internal Object
---
#### phone:

The *phone* object contains information about an individual phone and service.  Note that only one service is allowed per phone; so if multiple services are available on a number (e.g. mobile, sms, message) the phone object will need to be repeated.

__phone:__
````ruby
    def newPhone
        intObj = {
            phoneServiceType: nil,
            phoneName: nil,
            phoneNumber: nil
        }
    end
````

__phoneServiceType:__ *string* - a user provided description of the phone service  (e.g., voice, fax, or sms).

__phoneName:__ *string* - an open text field to describe the phone (e.g., 'main office' or 'Joe's mobile').

__phoneNumber:__ *alphaNumeric* - the phone number.  No format for the phone number is enforced.
