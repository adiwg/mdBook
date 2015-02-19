# Writer Functions

An mdTranslator writer formats the metadata content placed in the internal object by the reader into a properly formatted metadata record.

Most content rules are associated with a metadata standard and vary greatly between standards.  For this reasons it is the responsibility of the writer to decide how to handle missing or improperly formatted content found in the intern object.  Each writer may take a different approach to handling exceptions.  E.g. in ISO 19115-2 a missing required element will set a tag attribue nilReason='missing'. In this was the metadata record remains valid even with a required value missing.  
