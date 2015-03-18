# legalCon:

The *legalCon* object containing the various legal constraints regarding access and use of the resource.

````ruby
    def newLegalCon
        intObj = {
            accessCons: [],
            useCons: [],
            otherCons: []
        }
    end
````

__accessCons:__ *array* - an array of quoted strings statements identifying the various access constraints applied to the resource to assure protection of privacy or intellectual property, and any special restrictions or limitations on obtaining the resource or metadata

__useCons:__ *array* - an array of quoted strings statements identifying the various constraints applied to assure protection of privacy or intellectual property, and any special restrictions or limitations or warnings on using the resource or metadata

__otherCons:__ *array* - an array of quoted strings statements identifying other restrictions and legal prerequisites for accessing and using the resource or metadata
