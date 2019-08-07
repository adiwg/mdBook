# mdTranslator

## Extending the mdTranslator

### Rules for Readers

````ruby
class Option
	def self.getOptionList
		hOptions = {
			readers: %w[mdJson {new reader}],
			writers: %w[iso19115_2 iso19110 html],
````
.2. Add a link to the new Reader's web page.  The page will be dynamically built by the Rails application.  It's content will be the content of the readme.md file placed in the Reader's root folder (see step 7 above). Below is the example for Reader mdJson.

````md
 [mdJson](./readers/mdJson)

 : Alaska Data Integration working group JSON metadata format
````

