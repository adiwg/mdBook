# mdTranslator

## Add an XML Writer

### Setup

These guidelines assume that the developer has already forked the mdTranslator and is working in a branch other than "master" or "dev".

XML writers rely on building an XML formatted metadata file from the contents of the internal object using the "builder" gem.  The "builder" gem is installed with mdTranslator.  Require the gem:
```ruby
require 'builder'
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
         end 
      end
     ````

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
  
1. Create the writer's initial module.  
   * Purpose:
      * Setup message processing.
      * Setup builder to write the XML metadata file.
      * Set hResponseObj writer elements.
      * Call the initial (high level) build method.
      * Return the results of the build and the response hash, to the user. 
   * File path: /lib/adiwg/mdtranslator/writers/{writer_name}/
   * File name: {writer_name}_writer.rb 
   * Receiving method: 
     ````ruby
      def self.startWriter(intObj, hResponseObj)
         # code ...
      end 
     ````
   * Responsibilities:
      * Load the message file to a hash.
        ````ruby
         # load error message array
         file = File.join(File.dirname(__FILE__), '{writer_name}_writer_messages_eng') + '.yml'
         hMessageList = YAML.load_file(file)
        ````
      * Instance the message file path for error methods.
        ````ruby
         @aMessagesList = hMessageList['messageList']
        ````
      * Set hResponseObj[:writerOutputFormat] = 'json'
      * Set hResponseObj[:writerVersion] from version file
        ````ruby
         hResponseObj[:writerVersion] = ADIWG::Mdtranslator::Writers::{writer_name}::VERSION
        ````
      * Create a new XML document for the metadata output
        ````ruby
         # create new XML document
         @xml = Builder::XmlMarkup.new(indent: 3)
        ````  
      * Instance the initial (high-level) build module.  Pass in the new XML document and response hash.
        ````ruby
         # start writing the XML record
         metadataWriter = Fgdc.new(@xml, responseObj)
        ````        
      * Call the "writeXML" method of the initial build module. 
        ````ruby
         metadata = metadataWriter.writeXML(intObj)
        ````
      * Return the XML document to the user.
        ````ruby
         return metadata
        ````
      {% hint style='tip' %}
 The high-level build module will control the build process and receive the complete XML metadata file.
      {% endhint %}
      * Write the error handling methods to be used while unpacking elements.  You can view other readers for examples of necessary functionality.  In general readers should be relaxed in regard to throwing errors.  Warnings should be issued rather than errors unless there are serious issues.
         * loadMessages
         * findMessage
         * issueError
         * issueWarning
         * issueNotice
      {% hint style='tip' %}
 The mdJson writer does not set many error messages.  The primary purpose of the mdJson format is to support mdEditor.  As such, partial records are often saved, reloaded, or shared.  Therefore strict adherence to the standard is not enforced.
      {% endhint %}
      * Act as a container for any other methods that will be common to many or all metadata build modules. <br><br>

1. Create a 'classes' directory to hold the writer's build modules.  For flexibility create a separate build module for each object in the metadata standard.  This simplifies writing, maintenance, and permits reuse of the modules during unpacking.
   * Path: /lib/adiwg/mdtranslator/writers/{writer_name}/classes/ <br><br>
   
1. Create the initial (high level) build module. 
   * Purpose:
      * Receive control from {writer_name}_writer.rb, this file was created in the first coding step.
      * Build the XML header
      * Build the body framework and high-level metadata tags.
      * Control the build process for lower levels of the record.
   * File path: /lib/adiwg/mdtranslator/writers/{writer_name}/classes/
   * File name: {writer_name}_{writer_name}.rb 
   * Responsibilities:
      * Initialize method: Receive and instantiate the XML document and response hash for other methods in this class.  Include the namespace for error methods and any other method that are to be generally available.
        ````ruby
          def initialize(xml, hResponseObj)
             @xml = xml
             @hResponseObj = hResponseObj
             @NameSpace = ADIWG::Mdtranslator::Writers::Iso19115_1
          end
        ````
      * Build method: 
        ````ruby
          def writeXML(intObj)
             # code ...
          end
        ````
      * Add document head.  Example:
        ````ruby
         # document head
         metadata = @xml.instruct! :xml, encoding: 'UTF-8'
         @xml.comment!('ISO 19115-1 METADATA')
         @xml.comment!('The following metadata file was constructed using the ADIwg mdTranslator, http://mdtranslator.adiwg.org')
         @xml.comment!('mdTranslator software is an open-source project of the Alaska Data Integration working group (ADIwg)')
         @xml.comment!('mdTranslator and other metadata tools are available at https://github.com/adiwg')
         @xml.comment!('ADIwg is not responsible for the content of this metadata record')
         @xml.comment!('This metadata record was generated by mdTranslator ' + version + ' at ' + Time.now.to_s)
        ````
      * Add XML namespace tags if XSD is available.  Example:
        ````ruby
         # MD_Metadata
         @xml.tag!('mdb:MD_Metadata',
                  {
                   'xmlns:xsi' => 'http://www.w3.org/2001/XMLSchema-instance',
                   'xmlns:xlink' => 'http://www.w3.org/1999/xlink',
                   'xmlns:gml' => 'http://www.opengis.net/gml/3.2',
        ````
        
1. Write a separate build method for each XML metadata object.  There can be a lot of flexibility in coding the build modules.  However, I suggest staying with one theme throughout the reader to improve coding speed and maintenance.  
   * Purpose:
      * build the metadata object from mdTranslator's internal object.  This is most often straight forward, however sometimes it can get convoluted or even impractical.  
        {% hint style='tip' %}
 The internal object structure is closely patterned after ISO 19115-1.  Export from the internal object thus involves some amount of translation from the writer's metadata format to ISO 19115-1.
        {% endhint %}
      * Identify errors, problems with the output and report these to the user. 
   * Receiving method parameters (internal object block, response hash, in context).  Pass in only the portion of the internal object that is being translated by this module:
     ````ruby
     def self.writeXML(hInternalObjectBlock, inContext = nil)
         # code ...
     end
     ````
   * Responsibilities:
   
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
      * build the XML file for the writer standard.
          * __element example__:
            ````ruby
             # bounding box - west longitude (required)
             unless hBBox[:westLongitude].nil?
                @xml.tag!('gex:westBoundLongitude') do
                   @xml.tag!('gco:Decimal', hBBox[:westLongitude])
                end
             end
             if hBBox[:westLongitude].nil?
                @NameSpace.issueError(10)
             end
            ````
          * __class example__:
            ````ruby
             # data identification - citation {CI_Citation} (required)
             hCitation = hResource[:citation]
             unless hCitation.empty?
                @xml.tag!('mri:citation') do
                   citationClass.writeXML(hCitation, 'main resource')
                end
             end
             if hCitation.empty?
                @NameSpace.issueWarning(50, 'mri:citation')
             end
            ````
          * __array example__:
            ````ruby
             # data identification - credit []
             aCredits = hResource[:credits]
             aCredits.each do |credit|
                @xml.tag!('mri:credit') do
                   @xml.tag!('gco:CharacterString', credit)
                end
             end
             if aCredits.empty? && @hResponseObj[:writerShowTags]
                @xml.tag!('mri:credit')
             end
            ````
                  
   * __Comment__ - The comments preceding an build block describe where the build element fits in the XML metadata schema and has the following format:
      * {object being build} - {element being built (which could be an object)} {object type if it is an object} {[] if an array} {(required) if required}. <br><br>
         
   * __Testing__ - All element and object are tested as they are queried from the internal object and any unexpected status reported via the response hash. 
      * Test for empty and missing required objects.
      * The testing code is isolated to a separate block immediately below the unpacking block.  This makes the tests easy to find and maintain.  Decisions can be made based on the build status, showAllTags, and status of other build elements or objects as required.   

### Testing 

Testing the writer is done by sending complete mdJson metadata records to mdTranslator and requesting translation to the writer to be tested, then compare the actual results against previously validated metadata records or segments.  The tests should cover all possible variations; elements with values, elements without values, invalid values, missing elements, empty arrays, arrays with single element, arrays with multiple elements, etc. All situations that throw error messages should also be tested to see the proper error message is reported and no additional or distracting messages are included.  And remember to check that the message context is appropriate.

Ruby minitest is used to perform the tests. 

For mdTranslator writers, pass an mdJson metadata record to mdTranslator and request translation to the writer to be tested.  When mdJson metadata is read by mdTranslator it will pass through a validation process which rejects invalid records.  Although the mdJson must be valid it does not need to be comprehensive.  Add detail only for the metadata object being tested.  

The best, and easiest, method for building the mdJson test files is to generate them dynamically using the mdJson construction helpers in "/test/helpers".  In one step you can create your valid base metadata record:
````ruby
 require_relative '../../helpers/mdJson_hash_objects'
 require_relative '../../helpers/mdJson_hash_functions'

 # build mdJson test file in hash
 TDClass = MdJsonHashWriter.new
 mdHash = TDClass.base
````
In another steps add a fully populated blocks of data to meet your specific test requirements.
````ruby
 mdHash[:metadata][:resourceInfo][:citation] = TDClass.citation_full
````
{% hint style='tip' %}
  Another advantage is that when an object's schema changes and the helper is updated, no changes are required to the tests to assess the impact of the changes, unless of course the change breaks the code or requires additional tests.
{% endhint %}

1. Create a folder for the writer's test code.
   * Folder path: /test/writers/.
   * Folder name: must be the name of the writer.  <br><br>
   
1. Add a new folder for test data files if needed.  A test data file holds segments of metadata or full metadata records that will be processed by the writer and checked for expected or unexpected results.
   * Folder path: /test/writers/{writer name}/.
   * Folder name: suggest "testData".  <br><br>
   {% hint style='tip' %}
 Most test scripts will be built using mdJson construction helpers discussed above.  But occasionally a metadata file of special construction will be needs and it can be placed here.
   {% endhint %}
  
1. Add a parent test file to hold common tasks for all tests if useful.  Methods to read and parse test data files and load components common to all tests can be placed in this parent method.
   * File path: /test/writers/{writer name}/.
   * File name: {writer name}_test_parent.rb.  <br><br>
   
1. Write the XML test data first.  If you have an XSD use XMLSpy, Oxygen or similar tool to validate the test data before saving it in a test file.  In this way you are only comparing against validated metadata. The test data file also serves as an excellent pattern while coding the writer.  
   
1. Name each test module using the following pattern: "tc_{writer name}_{object name}.rb".  This will ensure rake will include your test module when running tests.  

1. Write tests.  You can view examples from other writers, but there are no requirements in writing the tests other than to be thorough. 

1. Use Nokogiri XPath to extract segments for the minitests.  There is no need to compare the entire returned metadata file against a full file in testData; and that would create many problems in itself.  Save only the validated clip to be compared against in the testData file and extract the clip to test from the result metadata using Nokogiri XPath.  

   These are a few methods added to the XML writer's parent test file.  'get_xml' handles loading the XML reference XML and 'run_test' handles extracting XML segments using Nokogiri XPath.  Note that before the minitest is performed the white space needs to be squeezed out the XML strings.

  ````ruby
   def self.get_xml(fileName)
      file = File.join(File.dirname(__FILE__), 'testData', fileName) + '.xml'
      xDoc = Nokogiri::XML(File.read(file))
      return xDoc
   end

   def self.run_test(hIn, expectFile, expectPath, gotPath, gotSuffix = 0)

      # read the fgdc reference file
      xFile = get_xml(expectFile)
      xExpect = xFile.xpath(expectPath)
      expect = xExpect.to_s.squeeze(' ')

      hResponseObj = ADIWG::Mdtranslator.translate(
         file: hIn.to_json, reader: 'mdJson', writer: 'iso19115_1', showAllTags: true, validate: 'none'
      )
      pass = hResponseObj[:writerPass] &&
         hResponseObj[:readerStructurePass] &&
         hResponseObj[:readerValidationPass] &&
         hResponseObj[:readerExecutionPass]

      xMetadata = Nokogiri::XML(hResponseObj[:writerOutput])
      xGot = xMetadata.xpath(gotPath)[gotSuffix]
      got = xGot.to_s.squeeze(' ')

      return expect, got, pass, hResponseObj[:writerMessages]

   end
  ````

1. Run "rake" to test run all tests.  While building a writer you can comment out lines in "Rakefile" to exclude other readers and writers.  Before declaring completion, be sure to reactivate all reader and writer tests and then test all together to be sure the new reader did not introduce unanticipated errors.
