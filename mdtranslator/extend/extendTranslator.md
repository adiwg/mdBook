# mdTranslator

## Extending the mdTranslator

New readers and writers can be added with without impact to the base mdTranslator code.  And care should always be taken to construct new readers and writers in a way that will not interfere with existing readers, writers, and base modules.  Following the guidelines in this section will lead you to developing new code that will have minimal impact on the existing code and structure.  

A developer of a new reader or writer should good working knowledge of the following:

* Ruby programming language 2.5.1 or higher

* an understanding of the architecture of mdTranslator's base code

* HTML

* JSON structure

* GeoJSON format for geographic objects

* mdTranslator internal object format

* Ruby minitest

* Git and GitHub

* have a suitable IDE 

* Ruby 'builder' GEM for XML writers

* Nokogiri XPath for XML readers and writers

* XSD and XMLSpy or equivalent for XML readers and writers

* jBuilder for JSON writers

* JSON Schema for JSON readers

* markdown

* and, of course, a solid understanding of the reader or writer standard being added to mdTranslator.  

New development should always be done in a remote branch of mdTranslator.  So start by forking the mdTranslator repo.

[__Fork the Reposotory__](forkRepository.md) - covers creating a personal copy fo the mdTranslator code library for your personal use or to develop new extensions, readers, and/or writers.

[__mdTranslator base Architecture__](folderStructure.md) - covers the mdTranslator methods and work flow.  

[__Adding Readers__](addReadWrite.md) - how to add a new mdTranslator reader. 

[__Adding Writers__](creatingWriters.md) - how to add a new mdTranslator writer. 
