# onlineResource:

The *onlineResource:* array holds links and other information to a contact's (indiviual or organization) resources exposed on the internet.

````ruby
    def newOnlineResource
        intObj = {
            olResURI: nil,
            olResProtocol: nil,
            olResName: nil,
            olResDesc: nil,
            olResFunction: nil
        }
    end
````

__olResURI:__ *string* - a Universal Resource Identifier (URI) for the online resource.  May be either a Uiversal Resource Locator (URL) or Universe Resource Name (URN).  The URI generally points to a web page, website, or online service,

__olResProtocol:__ *string* - the protocol supported by the URI; e.g. http, ftp.

__olResName:__ *string* - a user supplied name for the URI.

__olResDesc:__ *string* - a short description of the URI.

__onResFunction:__ *string* - the purpose of the online resource; e.g. information, data.
