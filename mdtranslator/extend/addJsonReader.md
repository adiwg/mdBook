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
      * Return the results of the unpack, the response hash, to the user. 
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/
   * File name: {reader_name}_reader.rb 
   * Receiving method: 
   ````ruby
   def self.readFile(file, hResponseObj)
      # code ...
   end 
   ````
   * Responsibilities:
      * Parse the input JSON file to a hash {hash_file_name}.
      * Set hResponseObj[:readerStructureMessages] if problems found.
      * Set hResponseObj[:readerStructurePass] to 'false' if problem.
      * Set hResponseObj[:readerVersionRequested]. 
      * Set hResponseObj[:readerVersionUsed]. 
      * Call JSON schema validation method if written.
      * Set hResponseObj[:readerValidationPass] to 'false' if problem. 
      * Call the reader's initial 'unpack' method.
      ````ruby
        # unpack the mdJson into the internal object
        return {Reader_name}.unpack({hash_file_name}, hResponseObj)
      ````

1. Create a 'modules' directory to hold the reader's unpacking modules.  For flexibility create a separate unpacking module for each class or object in the metadata standard.  This simplifies writing, maintenance, and permits reuse of the modules during unpacking.
   * Path: /lib/adiwg/mdtranslator/readers/{reader_name}/modules/ <br><br>
   
1. Create the initial (high level) unpacking module. 
   * Purpose:
      * Receive control from {reader_name}_reader.rb, this file was created in the first coding step.
      * Create a new instance of the internal object (data store) to hold the results of the read operation.
      * Hold other methods used by multiple of the reader's lower level unpack modules.
      * Unpack the top level of the input metadata into the internal object, 'intObj'.
      * Send the results of the read back to the user.
   * File path: /lib/adiwg/mdtranslator/readers/{reader_name}/modules/
   * File name: module_{reader_name}.rb 
   * Receiving method: 
     ````ruby
     def self.unpack({hash_file}, hResponseObj)
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
      * Write error handling methods to use while unpacking elements.  See other readers for examples of necessary functionality.
         * loadMessages
         * findMessage
         * issueError
         * issueWarning
         * issueNotice
      * Add other methods that will be used all or many of the reader's other unpack methods, such as 'findContact'. 
      * Unpack the high level of {hash_file} into the internal object, intObj. Unpacking the highest level of the {hash_file} follows the same logic as unpacking any lower level of the JSON hash which is described below.<br><br>
      
1. Write a separate unpack method for each class or object to be unpacked.  There can be a lot of flexibility in coding the unpacking modules.  However, I suggest staying with one theme throughout the reader to improve coding speed and maintenance.  
   * Purpose:
      * Unpack the object's elements from the input metadata and translate them into the internal object's structure.  This is most often straight forward, however sometimes it can get convoluted or even impractical.  
      * Identify errors, problems with the input and report these to the user. 
   * Receiving method parameters (object to unpack, response hash, in context):
     ````ruby
     def self.unpack(hCitation, responseObj, inContext = nil)
         # code ...
     end
     ````
   * Responsibilities:
      * Set a path to the location of the error methods and any other general purpose reader methods.  Example:
        ````ruby
        @MessagePath = ADIWG::Mdtranslator::Readers::MdJson::MdJson
        ````
      * Test if the input object exists, else issue warning and return nil.  Example:
         ````ruby
         # return nil object if input is empty
         if hCitation.empty?
            @MessagePath.issueWarning(80, responseObj, inContext)
            return nil
         end
         ````
      * Construct an 'outContext' message to be used in error messages.  Use the inContext if present.  The inContext will describe the parent object of the current object being unpacked thus allowing a means of preserving a path.  Example:
         ````ruby
         outContext = 'citation'
         outContext = inContext + ' > ' + outContext unless inContext.nil?

         ````
      * Unpack the object's elements into a local hash constructed from "/lib/adiwg/mdtranslator/internal/internal_metadata_obj.rb" methods.  Example: 
         ````ruby
         intMetadataClass = InternalMetadata.new
         intAdd = intMetadataClass.newAddress
         ````
      * Pass objects to that object's unpacking method.  Test that returned unpacked objects are valid before adding them into the local hash.  Example:
         ````ruby
         # contact - address [address]
         if hContact.has_key?('address')
             hContact['address'].each do |item|
               hReturn = Address.unpack(item, responseObj, outContext)
               unless hReturn.nil?
                  intContact[:addresses] << hReturn
               end
            end
         end
         ````
   Here are some examples from the mdJson reader:

   __Unpack element__...
   ````ruby
      # address - description 
      if hAddress.has_key?('description')
        unless hAddress['description'] == ''
           intAdd[:description] = hAddress['description']
        end
     end
   ````
   
   __Unpack array__...
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
   
   __Unpack object__...
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
   
   * __Comment__ - The comments preceding an unpacking block describe where the element fits in the input metadata schema and has the following format:
      * {object being unpacked} - {element being unpacked (which could be an object)} {object type if it is an object} {[] if an array} {(required) if required}.  In 'Unpack array' example above:
         * 'mdJson' is the object being unpacked; 
         * 'contact' is the 'mdJson' element being unpacked which happens to be an array of objects of type 'contact'.
         * The 'contact' object is required by the by the mdJson standard.
         
   * __Testing__ - All element and object are tested as they are unpacked and any unexpected status reported via the response hash. 
      * Test for empty and missing objects to avoid system and application error during processing.
      * The testing code is isolated to a separate block immediately below the unpacking block.  This makes the tests easy to find and maintain.  Decisions can be made based on the unpack status, showAllTags, and status of other unpacked elements or objects as required.   

### Testing 

1. 


### Publish

1. Add to Rails API

1. Add to HTML writer

1. Bump version number

1. Pull requests