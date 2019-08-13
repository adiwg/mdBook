# mdTranslator

## Add a XML Reader

### Setup

These guidelines assume that the developer has already forked the mdTranslator and is working in a branch other than "master" or "dev".

XML readers rely on converting the XML input file to an XPath file in Nokogiri format to do the reads.  The "nokogiri" gem is required for this operation and already install with mdTranslator.  Require the gem:
```ruby
require 'nokogiri'
```

1. Name the reader
   * The reader name should be a single word or mnemonic using only lowercase letters, numbers, and the underscore ( _ ).
   * The reader name must be unique among readers, but may be the same as a writer.
   * The reader name, with first letter capitalized, will be used to qualify the namespace for all reader files as follows:
   
   ````ruby
   module ADIWG
      module Mdtranslator
         module Readers
            module ReaderName

               module ReaderModule
                  def self.doSomething()
                     # code...
                  end

   ````
   * Reader module names may be named as needed. <br><br>
   
1. Create a folder for the reader code.
   * The reader folder will be in /lib/adiwg/mdtranslator/readers/.
   * The reader folder name must be the name of the reader.  <br><br>
   
1. Add the reader name to the CLI 'reader' parameter's enumeration list.
   * File: /lib/adiwg/mdtranslator_cli.rb
   * Code:
   ````ruby
   method_option :reader, :aliases => '-r', :desc => 'Reader to read your input metadata file',
                 :enum => %w{mdJson sbJson fgdc}, :required => true
   ````
   
1. Create a README file for the reader.  This file will be accessed by the mdTranslator API and website.  Include the origin and history of the metadata standard and links to any reference websites. 
   * Written in markdown.
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/
   * File name: readme.md
   * Template:
   ````markdown
     ## {reader_name}

     ### Supported versions

     > 2.x (example)

     ### Reader for {metadata standard} metadata format (reader_name)

     Text goes here... 
   ````

1. Create a version file for the reader.  This file will be accessed by the mdTranslator API, website, and writer.  This sets the current version of the reader. 
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/
   * File name: version.rb
   * Template:
   ````ruby
    # adiwg / mdTranslator / readers / {reader_name}
    
    # {version} {date} {action}
    
    module ADIWG
       module Mdtranslator
          module Readers
             module {Reader_name}
                VERSION = '0.0.0'
             end
          end
end   ````

1. Add the file for reader messages. 
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/
   * File name: {reader_name}_reader_messages_eng.yml 
   * File name should include language in which the messages are written.  Always include english, other languages when international support is added. 
   * Messages are coded in YAML.
   * Template:
   ````yaml
    # Reader messages for {reader_name} {version}
    
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
      * Receive control from the 'translate' method.
      * Validate the input file is structurally sound, is in the appropriate format, and of a version to be handled by the reader.
      * Call the initial (high level) unpack method.
      * Return the results of the unpack and the response hash, to the user. 
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/
   * File name: {reader_name}_reader.rb 
   * Receiving method: 
   ````ruby
   def self.readFile(file, hResponseObj)
      # code ...
   end 
   ````
   * Responsibilities:
      * Test that the XML file is well formed by converting the XML file to a Nokogiri XPath document.  The Nokogiri document will be referenced as "xDoc" throughout this document.
      ````ruby
       begin
          xDoc = Nokogiri::XML(file) { |form| form.strict }
       rescue Nokogiri::XML::SyntaxError => err
          hResponseObj[:readerStructureMessages] << 'ERROR: XML file is not well formed'
          hResponseObj[:readerStructureMessages] << err.to_s
          hResponseObj[:readerStructurePass] = false
          return {}
       end
      ````
      * Set hResponseObj[:readerStructureMessages] if problems found.
      * Set hResponseObj[:readerStructurePass] to 'false' if problem.
      * Set hResponseObj[:readerVersionRequested]. 
      * Set hResponseObj[:readerVersionUsed]. 
      * Call XML schema validation method if written.
      * Call the reader's initial 'unpack' method.
      ````ruby
        # unpack the Nokogiri xPath document into the internal object
        return {reader_name}.unpack(xDoc, hResponseObj)
      ````

1. Create a 'modules' directory to hold the reader's unpacking modules.  For flexibility create a separate unpacking module for each object of object in the metadata standard.  This simplifies writing, maintenance, and permits reuse of the modules during unpacking.
   * Path: /lib/adiwg/mdtranslator/readers/{reader_name}/modules/ <br><br>
   
1. Create the initial (high level) unpacking module. 
   * Purpose:
      * Receive control from {reader_name}_reader.rb, this file was created in the first coding step.
      * Create a new instance of the internal object (data store) to hold the results of the read operation.
      * To contain other methods used by multiple of the reader's lower level unpack modules.
      * Unpack the top level of the input metadata into the internal object, 'intObj'.
      * Send the results of the read back to the user.
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/modules/
   * File name: module_{reader_name}.rb 
   * Receiving method: 
     ````ruby
     def self.unpack({xDoc}, hResponseObj)
        # code ...
     end 
     ````
   * Responsibilities:
      * Load the message file to a hash.
      * Instance the message file path.
      * Create a new hash for the internal object (data store) named 'intObj' using 'intMetadataClass' methods.  Example:
         ````ruby
          intMetadataClass = InternalMetadata.new
          intObj = intMetadataClass.newBase
         ````
      * Instance the internal object and other variables for use in instance methods:
      ````ruby
       @intObj = intObj
       @contacts = intObj[:contacts]
       @xDoc = xDoc
      ````
      * Write the error handling methods to be used while unpacking elements.  You can view other readers for examples of necessary functionality.  In general readers should be relaxed in regard to throwing errors.  Warnings should be issued rather than errors unless there are serious issues.
          * loadMessages
          * findMessage
          * issueError
          * issueWarning
          * issueNotice
      * Add additional methods that can be used all or many of the reader's other unpacking methods, such as 'findContact'.  These may not be apparent until you are well into coding the reader.  
      * Unpack the high level of {xDoc} into the internal object, intObj. Unpacking the highest level of the {xDoc} follows the same logic as unpacking any lower level of the Nokogiri XPath document which is described below.<br><br>
      
1. Write a separate unpack method for each object to be unpacked.  There can be a lot of flexibility in coding the unpacking modules.  However, Nokogiri XPath rules must be observed and I suggest staying with one theme throughout the reader to improve coding speed and maintenance.  
    * Purpose:
       * Unpack the object's elements from the input metadata and translate them into the internal object's structure.  This is most often straight forward, however sometimes it can get convoluted or even impractical. 
      {% hint style='tip' %}
 The internal object structure is closely patterned after ISO 19115-1.  Import to the internal object thus involves some amount of translation from the reader's metadata format to ISO 19115-1.
      {% endhint %}
       * Identify errors, problems with the input and report these to the user. 
    * Receiving method parameters (XPath object to unpack, response hash, in context):
     ````ruby
      def self.unpack(xCitation, hResponseObj, inContext)
         # code ...
      end
     ````
    * Responsibilities:
       * Set a path to the location of the error methods and any other general purpose reader methods.  Example:
        ````ruby
         require_relative 'module_fgdc'
        ````
       * Construct an 'outContext' message to be used in error messages.  Use the inContext if present.  The inContext will describe the parent object of the current object being unpacked thus allowing a means of preserving a path.  Example:
         ````ruby
         outContext = 'citation'
         outContext = inContext + ' > ' + outContext unless inContext.nil?

         ````
       * Unpack the object's elements into a local hash constructed from "/lib/adiwg/mdtranslator/internal/internal_metadata_obj.rb" methods.  Example: 
         ````ruby
         intMetadataClass = InternalMetadata.new
         hCitation = intMetadataClass.newCitation
         ````
       * Unpack objects by sending them to that object's unpacking method.  Test that returned unpacked objects are valid before adding them into the local hash.  Example:
         ````ruby
          # citation 8.8 (pubinfo) - publication information
          xPublication = xCiteInfo.xpath('./pubinfo')
          unless xPublication.empty?
             hResponsibility = Publication.unpack(xPublication, hResponseObj)
             unless hResponsibility.nil?
                hCitation[:responsibleParties] << hResponsibility
             end
          end
         ````
   Here are some examples from the FGDC reader:

   __Unpack element__...
   ````ruby
    # citation 8.4 (title) - citation title (required)
    title = xCiteInfo.xpath('./title').text
    unless title.empty?
       hCitation[:title] = title
    end
    if title.empty?
       hResponseObj[:readerExecutionMessages] << 'WARNING: FGDC reader: citation title is missing'
    end
   ````
   
   __Unpack array__...
   ````ruby
    # citation 8.10 (onlink) - online linkage []
    axOnLink = xCiteInfo.xpath('./onlink')
    unless axOnLink.empty?
       description = 'Link to the resource described in this citation'
       axOnLink.each do |xLink|
          onLink = xLink.text
          unless onLink.empty?
             hURI = OnlineResource.unpack(onLink, description, hResponseObj)
             unless hURI.nil?
              hCitation[:onlineResources] << hURI
             end
          end
       end
    end
   ````
   
   __Unpack object__...
   ````ruby
    # citation 8.11 (lworkcit) - larger work citation
    xLWCitation = xCiteInfo.xpath('./lworkcit')
    unless xLWCitation.empty?
       hLWCitation = Citation.unpack(xLWCitation, hResponseObj)
       unless hLWCitation.nil?
          hAssResource = intMetadataClass.newAssociatedResource
          hAssResource[:associationType] = 'largerWorkCitation'
          hAssResource[:resourceCitation] = hLWCitation
          Fgdc.add_associated_resource(hAssResource)
       end
    end
   ````
   
   * __Comment__ - The comments preceding an unpacking block describe where the element fits in the input metadata schema and has the following format:
      * {object being unpacked} - {element being unpacked (which could be an object)} {object type if it is an object} {[] if an array} {(required) if required}.  In 'Unpack array' example above:
         * 'citation' is the object being unpacked; 
         * '8.11 (lworkcit) - larger work citation' is the 'fgdc' element being unpacked.
         
   * __Testing__ - All element and object are tested as they are unpacked and any unexpected status reported via the response hash. 
      * Test for empty and missing objects to avoid system and application error during processing.
      * The testing code is isolated to a separate block immediately below the unpacking block.  This makes the tests easy to find and maintain.  Decisions can be made based on the unpack status, showAllTags, and status of other unpacked elements or objects as required.   

### Testing 

Testing the reader is done by sending known metadata records or metadata segments to a reader module and testing that the expected results are achieved.  All variations should be tested, elements with values, without values, invalid values, missing elements, empty arrays, arrays with single element, arrays with multiple elements, etc. All situations that throw error messages should be tested to see the proper error message is reported and no other messages that may re redundant or confusing.  Also check that the message context is appropriate.

Ruby minitest is used to help perform the tests.  

For mdTranslator readers, its practical to test each reader module independently.  This means the test data file only needs to pass in the metadata segment the metadata module will process, not a full metadata record.  

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
