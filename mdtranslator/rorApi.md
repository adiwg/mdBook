# mdTranslator

## Architecture

### GET verb

 * __.../api/v1/translator?{options}__ # returns metadata from the mdTranslator according to options specified
   - accepts requests with options encoded as key-value pairs in the query string.
   - only recommended for use when JSONp is required, i.e. for clients without CORS support.
   - **Note**: subject to URI size limits

### POST verb

 * __.../api/v1/translator?{options}__ # returns metadata from the mdTranslator according to options specified
   - accepts *application/x-www-form-urlencoded* requests with options encoded as key-value pairs.

### POST Options
> __file__ (string) *required*
 : the input file to be translated by mdTranslator.<br>
    the format of the file must be provided in the 'reader=' option.
>
> __reader__= (string) *required*
 : specifies a reader for the mdTranslator
>
> __writer__= (string)
 : specifies a writer for the mdTranslator; <br> a null writer will validate input only
>
> __validate__= [none | __normal__ | strict]
 :
>
>> __none__
>> : the input is not validated
>>
>> __normal__
>> : the input must meet the structural rules for the file format; <br>
    the input must meet the minimum rule set defined by the reader schema
>>
>> __strict__
>> : the input must meet the structural rules for the file format; <br>
    the input must meet the maximum rule set defined by the reader schema, all fields must have values
>
> __showAllTags__= [true | __false__]
 : show empty tags for all attributes that did not have values
>
> __format__= [__auto__ | plain | json | xml]
 :
>
>> __auto__
>> : content-type is set according to the writer; <br>
    if a writer was not specified the content-type will be set to 'text/plain'; <br>
    if validation errors prevent the writer from generating a return, messages will be returned as 'text/plain'; <br>
    if error messages are returned from the writer, a wrapper will be added with the content-type set according to the writer
>>
>> __plain__
>> : content-type="text/plain"; <br>
    return mdTranslator results in plain text; <br>
    if validation or translator messages are detected, only the messages will be returned
>>
>> __json__
>> : content-type="application/json" <br>
     results are placed in a JSON wrapper
>>
>> __xml__
>> : content-type="application/xml"; <br>
     results are placed in an XML wrapper
>
>
> __callback__= (string) default=null
> : when provided, a JSONp response if returned using the callback name provided; <br>
   - content-type is not set in the response header

