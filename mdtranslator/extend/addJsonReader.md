# mdTranslator

## Add a JSON Reader

### Setup

These guidelines assume that the developer has already forked the mdTranslator and is working in a branch other than "master" or "dev".

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
   * The reader folder must have the name of the reader.  <br><br>
   
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

When the 'translate' method is called for mdTranslator, the parameters are examined and control will be passed to the reader along with the input metadata file and the response hash.  The response hash will have the following elements populated by /lib/adiwg/mdtranslator.rb
  * hResponseObj[:readerRequested] = reader
  * hResponseObj[:readerValidationLevel] = validate
  * hResponseObj[:writerRequested] = writer
  * hResponseObj[:writerForceValid] = forceValid
  * hResponseObj[:writerShowTags] = showAllTags
  * hResponseObj[:writerCSSlink] = cssLink
  * hResponseObj[:translatorVersion] = ADIWG::Mdtranslator::VERSION
  
1. Create the initial module for the reader.  
   * Purpose:
      * Receive control from the 'translate' method.
      * To validate the input file is structurally sound and is the appropriate format and version to be read into the internal object (data store).
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/
   * File name: {reader_name}_reader.rb 
   * Receiving method: 
   ````ruby
   def self.readFile(file, hResponseObj)
      # code ...
   end 
   ````
   * Responsibilities:
      * Parse the file.json to a hash {hash_file_name}.
      * Set hResponseObj[:readerStructureMessages] if problems found.
      * Set hResponseObj[:readerStructurePass] if 'false'.
      * Set hResponseObj[:readerVersionRequested]. 
      * Set hResponseObj[:readerVersionUsed]. 
      * Call JSON schema validation if available.
      * Set hResponseObj[:readerValidationPass]. 
      * Call the reader's 'unpack' method.
      ````ruby
        # unpack the mdJson into the internal object
        return {Reader_name}.unpack({hash_file_name}, hResponseObj)
      ````

1. Create a 'modules' directory for the unpacking modules.  For flexibility create a separate unpacking module for each class or object in the metadata standard.  This simplifies writing, maintenance, and permits reuse of the module during unpacking.
   * Path: /lib/adiwg/mdtranslator/readers/{reader_name}/modules/ <br><br>
   
1. Add initial unpacking module.  This module receives the entire metadata hash and controls the unpacking of the metadata into the internal object (data store).
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/modules/
   * File name: module_{reader_name}.rb 
   * Receive control from {reader_name}_reader.rb
   * Receiving method: 
   ````ruby
   def self.unpack({hash_file}, hResponseObj)
      # code ...
   end 
   ````
   * Responsibilities:
      * Load the message file to hash
      * Instance the message path
      * Set up message handling routines to use while unpacking
         * loadMessages
         * findMessage
         * issueError
         * issueWarning
         * issueNotice
      * Create new instance of the internal object (data store)
      * Instance other useful objects such as 'contacts'
      * Unpack high level of {hash_file} 
      
1. Unpack the high-level class/object into internal object (data store).  There can be a lot of flexibility in coding the unpacking.  I would suggest staying with one theme throughout the reader to improve coding speed and maintenance.  Here are a few examples:

   Unpack element
   ````ruby
      # address - description 
      if hAddress.has_key?('description')
        unless hAddress['description'] == ''
           intAdd[:description] = hAddress['description']
        end
     end
   ````
   
   Unpack array
   ````ruby
      # mdJson - contact {contact} [] (required)
      if hMdJson.has_key?('contact')
         hMdJson['contact'].each do |hContact|
            hReturn = Contact.unpack(hContact, responseObj)
            unless hReturn.nil?
               intObj[:contacts] << hReturn
               @contacts = intObj[:contacts]
            end
         end
      end
      if intObj[:contacts].empty?
         @MessagePath.issueError(532, responseObj)
      end   
   ````
   
   Unpack object
   ````ruby
      # mdJson - schema {schema} (required)
      if hMdJson.has_key?('schema')
         hObject = hMdJson['schema']
         unless hObject.empty?
            hReturn = Schema.unpack(hObject, responseObj)
            unless hReturn.nil?
               intObj[:schema] = hReturn
            end
         end
      end
      if intObj[:schema].empty?
         @MessagePath.issueError(531, responseObj)
      end
   ````
   
   * Comment format shows the {object being unpacked} - {object element being unpacked (which could be an object)} {object type if object} {[] if array} {(required) if required}.
       * In the above example 'mdJson' is the object being unpacked.
       * 'schema' is the 'mdJson' element being unpacked which happens to be an object of type 'schema'.
       * The 'schema' object is required by the by the mdJson standard.
   * Test for empty and missing objects to avoid system and application error during processing.
   * Since 'schema' is an object it will be passed to the Schema.unpack method for unpacking.
   * If the returned object is valid, it is placed in the internal object.
   * All element and object unpacking steps are tested and unexpected status reported via the response object.  
   * The testing code is isolated from the unpacking block.  This makes the tests easy to find and maintain.  Decisions can be made based on the unpack status, showAllTags, and status of other unpacked elements or objects as required.

1. 

### Testing 

1. 


### Publish

1. Add to Rails API

1. Add to HTML writer

1. Bump version number

1. Pull requests