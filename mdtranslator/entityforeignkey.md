# entityForeignKey:

The *entityForeignKey* object defines a foreign key on the referencing (or child) entity in the form of a SQL ALTER TABLE, ADD CONSTRAINT statement.

````ruby
    def newEntityForeignKey
        intObj = {
            fkLocalAttributes: [],
            fkReferencedEntity: nil,
            fkReferencedAttributes: []
        }
    end
````

__fkLocalAttributes:__ *array* (required) - an array of quoted strings listing the local (referencing or child) attribute code names for this foreign key.

__fkReferencedEntity:__ *string* (required) - the entityID for the referenced (or parent) entity for this foreign key

__fkReferencedAttributes:__ *array* (required) - an array of quoted strings listing the referenced (or parent) attribute code names for this foreign key.  If the foreign key is compound key (more than one attribute compose the key) the order of the referenced attributes must allign precicely with the order and number of local attributes.
