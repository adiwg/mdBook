# mdTranslator

## Internal Object

The *internal object* is mdTranslator's internal data store and is implemented as a Ruby hash. The internal object is dynamically constructed in that arrays and objects are inserted into the hash only as the reader requires them.  

This does not mean the internal object is freely assembled.  The [mdJSON schema](https://mdtools.adiwg.org) website shows the current schema for mdJSON.  The internal object structure follows this schema very closely and only differs in a few element names.  The website thus becomes a good reference for the internal object as well as the mdJSON schema.

The "/lib/adiwg/mdtranslator/internal/internal_metadata_obj.rb" file has approximately 100 methods to construct each object supported by the mdJSON schema.  The objects are instanced by the reader, loaded with data, and inserted into their proper position in the internal object hash.  When building or reading an internal object, always start with the base object 'newBase()'.  The code for newBase() is shown below as an example of internal object construction methods.

````ruby
def newBase
      {
         schema: {},
         contacts: [],
         metadata: {},
         dataDictionaries: [],
         metadataRepositories: []
      }
   end
````
Newly instanced hash objects always set initial strings and numerics values to nil, arrays to empty [], and objects to empty {}.
