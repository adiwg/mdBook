# mdTranslator

## Add a JSON Writer

### Setup

These guidelines assume that the developer has already forked the mdTranslator and is working in a branch other than "master" or "dev".

JSON writers rely on building a JSON from the contents of the internal using the "jbuilder" gem.  The "jbuilder" gem is already install with mdTranslator.  Require the gem:
```ruby
require 'jbuilder'
```

1. Name the writer
   * The writer name should be a single word or mnemonic using only lowercase letters, numbers, and the underscore ( _ ).
   * The writer name must be unique among writer, but may be the same as a reader.
   * The writer name, with first letter capitalized, will be used to qualify the namespace for all writer files as follows:
   
   ````ruby
    module ADIWG
       module Mdtranslator
          module Writers
             module WriterModule
 
                  def self.doSomething()
                     # code...
                  end

   ````
   * Writer module names may be named as needed. <br><br>
   
1. Create a folder for the writer code.
   * The writer folder will be in /lib/adiwg/mdtranslator/writers/.
   * The writer folder name must be the name of the writer.  <br><br>
   
1. Add the writer name to the CLI 'writer' parameter's enumeration list.
   * File: /lib/adiwg/mdtranslator_cli.rb
   * Code:
   ````ruby
    method_option :writer, :aliases => '-w',
                 :desc => 'Writer to create your output metadata file, leave blank to validate input only',
                 :enum => %w{fgdc html iso19110 iso19115_1 iso19115_2 mdJson sbJson }
   ````
   
1. Create a README file for the writer.  This file will be accessed by the mdTranslator API and website.  Include the origin and history of the metadata standard and links to any reference websites. 
   * Written in markdown.
   * File path: /lib/adiwg/mdtranslator/writers/{writer_name}/
   * File name: readme.md
   * Template:
   ````markdown
     ## {reader_name}

     ### Supported versions

     > 2.x (example)

     ### Writer for {metadata standard} metadata format (writer_name)

     Text goes here... 
   ````

1. Create a version file for the writer.  This file will be accessed by the mdTranslator API, website, and writer.  This sets the current version of the writer. 
   * File path: /lib/adiwg/mdtranslator/writers/{writer_name}/
   * File name: version.rb
   * Template:
   ````ruby
    # adiwg / mdTranslator / writers / {writer_name}
    
    # {version} {date} {action}
    
    module ADIWG
       module Mdtranslator
          module Writers
             module {Writer_name}
                VERSION = '0.0.0'
             end
          end
end   ````

1. Add the file for writer messages. 
   * File path: /lib/adiwg/mdtranslator/writers/{writer_name}/
   * File name: {writer_name}_writer_messages_eng.yml 
   * File name should include language in which the messages are written.  Always include english, other languages when international support is added. 
   * Messages are coded in YAML.
   * Template:
   ````yaml
    # Writer messages for {writer_name} {version}
    
    # History:
    #  {your name} {date} {action}
    #  {your name} {date} original script
    
    messageList:
       - {id: 1, message: "message 1"}
       - {id: 2, message: "message 2"}
       - {id: 3, message: "message 3"}
   ````




### Coding 

When mdTranslator's 'translate' method is called, the parameters are examined and control passed to the reader along with the input metadata file and the response hash.  The response hash will have the following elements pre-populated by /lib/adiwg/mdtranslator.rb
  * hResponseObj[:readerRequested] = reader
  * hResponseObj[:readerValidationLevel] = validate
  * hResponseObj[:writerRequested] = writer
  * hResponseObj[:writerForceValid] = forceValid
  * hResponseObj[:writerShowTags] = showAllTags
  * hResponseObj[:writerCSSlink] = cssLink
  * hResponseObj[:translatorVersion] = ADIWG::Mdtranslator::VERSION
  
1. Create the reader's initial module.  
   * Purpose:
      * Setup jBuilder to write JSON metadata file.
      * Set hResponseObj writer elements
      * Call the initial (high level) build method.
      * Return the results of the unpack and the response hash, to the user. 
   * File path: /lib/adiwg/mdtranslator/writers/{writer_name}/
   * File name: {writer_name}_writer.rb 
   * Receiving method: 
   ````ruby
   def self.startWriter(intObj, hResponseObj)
      # code ...
   end 
   ````
   * Responsibilities:
      * Set the jBuilder flag to ignore empty elements if hResponse[:showAllTags] is "FALSE".
      ````ruby
       Jbuilder.ignore_nil(!responseObj[:writerShowTags])
      ````
      * Set hResponseObj[:writerOutputFormat] = 'json'
      * Set hResponseObj[:writerVersion] from version file
      ````ruby
       schemaVersion = Gem::Specification.find_by_name('adiwg-mdjson_schemas').version.to_s
       responseObj[:writerVersion] = schemaVersion
      ````
      * Call initial (high-level build module)
      ````ruby
       metadata = {Writer_name}.build(intObj, responseObj)
      ````
      {% hint style='tip' %}
 The high-level build module will control the build process and receive the complete JSON metadata file.
      {% endhint %}
      * Set hResponseObj[:writerPass] based on messages returned during build processes.
      ````ruby
       responseObj[:writerPass] = true if responseObj[:writerMessages].empty?
      ````
      * Write the error handling methods to be used while unpacking elements.  You can view other readers for examples of necessary functionality.  In general readers should be relaxed in regard to throwing errors.  Warnings should be issued rather than errors unless there are serious issues.
         * loadMessages
         * findMessage
         * issueError
         * issueWarning
         * issueNotice
      {% hint style='tip' %}
 The mdJson writer does not set many error messages.  The primary purpose of the mdJson format is to support mdEditor.  As such, partial records are often saved, reloaded, or shared.  Therefore strict adherence to the standard is not enforced.
      {% endhint %}
      * Act as a container for any other methods that will be common to many or all metadata build modules.  The following method will be useful to include if your metadata standard uses arrays:
      ````ruby
       # ignore jBuilder object mapping when array is empty
       def self.json_map(collection = [], _class)
          if collection.nil? || collection.empty?
             return nil
          else
             collection.map { |item| _class.build(item).attributes! }
          end
       end
      ````
      * Convert the jBuilder document to proper JSON format
      ````ruby
       metadata.target!
      ````

1. Create a 'modules' directory to hold the writer's build modules.  For flexibility create a separate build module for each object in the metadata standard.  This simplifies writing, maintenance, and permits reuse of the modules during unpacking.
   * Path: /lib/adiwg/mdtranslator/writers/{writer_name}/modules/ <br><br>
   
1. Create the initial (high level) build module. 
   * Purpose:
      * Receive control from {writer_name}_writer.rb, this file was created in the first coding step.
      * Create a new jBuilder document.
      * Initiate and build process.
      * Send complete jBuilder file to the user.
   * File path: /lib/adiwg/mdtranslator/writers/{writer_name}/modules/
   * File name: {writer_name}_{writer_name}.rb 
   * Receiving method: 
     ````ruby
      def self.build(internal object, hResponseObj)
         # code ...
      end 
     ````
  * Responsibilities:
      * Create a new jBuilder document
        ````ruby
         Jbuilder.new do |json|
            # code ... 
         end
        ````
      * Build JSON metadata file.
      
         __element example__
         ````ruby
          json.name 'mdJson'
         ````
         __element in block example__
         ````ruby
          json.schema do
             json.name 'mdJson'
             json.version hResponseObj[:writerVersion]
          end
         ````
         __array of objects example__
         ````ruby
          # mdJson - contacts [] (required)
          json.contact intObj[:contacts].map { |obj| Contact.build(obj).attributes! }
         ````
         __array of objects using json_map example__
         ````ruby
          json.responsibleParty @Namespace.json_map(hCitation[:responsibleParties], ResponsibleParty)
         ````
         {% hint style='tip' %}
 json_map is a method added to the startWriter method to handle empty arrays, see above.
         {% endhint %}
         
1. Write a separate build method for each JSON metadata object.  There can be a lot of flexibility in coding the build modules.  However, I suggest staying with one theme throughout the reader to improve coding speed and maintenance.  
   * Purpose:
      * build the metadata object from mdTranslator's internal object.  This is most often straight forward, however sometimes it can get convoluted or even impractical.  
        {% hint style='tip' %}
 The internal object structure is closely patterned after ISO 19115-1.  Export from the internal object thus involves some amount of translation from the writer's metadata format to ISO 19115-1.
        {% endhint %}
      * Identify errors, problems with the output and report these to the user. 
   * Receiving method parameters (internal object block, response hash, in context).  Pass in only the portion of the internal object that is being translated by this module:
     ````ruby
     def self.build(hInternalObjectBlock, responseObj, inContext = nil)
         # code ...
     end
     ````
   * Responsibilities:
      * Set a path to the location of the error methods and any other general purpose reader methods.  Example:
        ````ruby
        require_relative 'mdJson_writer'
        ````
      * Test if the input object exists, else issue warning and return nil.  Example:
         ````ruby
         # return nil object if input is empty
         if hCitation.empty?
            MdJson.issueWarning(80, responseObj, inContext)
            return nil
         end
         ````
      * Construct an 'outContext' message to be used in error messages.  Use the inContext if present.  The inContext will describe the parent object of the current object being unpacked thus allowing a means of preserving a path.  Example:
         ````ruby
         outContext = 'citation'
         outContext = inContext + ' > ' + outContext unless inContext.nil?
         ````
      * Build the JSON metadata object for the data found in the internal object block. 
            
   * __Comment__ - The comments preceding an build block describe where the build element fits in the JSON metadata schema and has the following format:
      * {object being build} - {element being built (which could be an object)} {object type if it is an object} {[] if an array} {(required) if required}.
         
   * __Testing__ - All element and object are tested as they are queried from the internal object and any unexpected status reported via the response hash. 
      * Test for empty and missing required objects.
      * The testing code is isolated to a separate block immediately below the unpacking block.  This makes the tests easy to find and maintain.  Decisions can be made based on the build status, showAllTags, and status of other build elements or objects as required.   

### Testing 

Testing the writer is done by sending complete mdJson metadata records to mdTranslator and requesting translation to the writer in question then comparing results against validated metadata records or segments.  All variations should be tested, elements with values, without values, invalid values, missing elements, empty arrays, arrays with single element, arrays with multiple elements, etc. All situations that throw error messages should be tested to see the proper error message is reported and no other messages that may re redundant or confusing.  Also check that the message context is appropriate.

Ruby minitest is used to help perform the tests. 

For mdTranslator writers, pass a mdJson metadata record to mdTranslator and request translation to the writer to be tested.  The Even though a full metadata record must be passed to mdTranslator.  

{% hint style='tip' %}
  mdJSON segments and files are used to test the mdJson reader.  They are also used to test all writers as well because only the mdJson format completely encompasses the internal object.  Because of the heavy use of mdJson files and scripts in testing and ensuing maintenance issues when changes are made to the mdJson schema, mdJson construction helpers were built and added to "/test/helpers/".  Thus there are no static mdJson reader test scripts.  All tests are generated dynamically from these helpers.  This tactic could be taken with other readers as well if the developer desires.  See "/test/helpers/mdJson_hash_objects.rb" and "/test/helpers/mdJson_hash_functions.rb" for ideas.
{% endhint %} 

1. Create a folder for the reader's test code.
   * Folder path: /test/readers/.
   * Folder name: must be the name of the reader.  <br><br>
   
1. Add a new folder for test data files if needed.  A test data file holds segments of metadata or full metadata records that will be processed by the reader and checked for expected results.
   * Folder path: /test/readers/{reader name}/.
   * Folder name: suggest "testData".  <br><br>
  
1. Add a parent test method to handle common tasks for all tests if useful.  Methods to read and parse test data files and load components common to all tests can be placed in this parent method.
   * File path: /test/readers/{reader name}/.
   * File name: {reader name}_test_parent.rb.  <br><br>
   
1. Name each test module using the following pattern: "tc_{reader name}_{object name}.rb".  This will ensure rake will include your test module when running tests.  

1. Write tests.  You can view examples for other readers, but there are no requirements in writing the tests other than to be thorough. 

1. Run "rake" to test run all tests.  While building a reader you can comment out lines in "Rakefile" to exclude other readers and writers.  Before declaring completion, be sure to reactivate all reader and writer tests and then test all together to be sure the new reader did not introduce unanticipated errors.
