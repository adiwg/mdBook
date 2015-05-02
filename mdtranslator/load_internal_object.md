# Reader Functions
## Load Internal Object

Once an input metadata file is determined to be valid it can be read into the mdTranslator's internal object.  The internal object is a Ruby hash which uses keys as symbols rather than the implicit form which uses strings as keys.

````ruby
schema = { name: 'mdJson', version: '1.0.1' }
schema[:name] #=> mdJson
````

All mdTranslator writers will access their metadata content from this hash.  See the [Internal Object](Internal Object) section for information on the structure of the internal hash.

The rationale to Load the metadata contents of the input file into an internal object rather to write directly to a metadata content standard allows the input format to be accessed by all of mdTranslator's Writers.


