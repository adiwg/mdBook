# mdTranslator

## Overview
The *mdTranslator* is the heart of the ISO Metadata Developer's Toolkit. The *mdTranslator* translates metadata content from any supported reader format into any of the supported writer formats.  The *mdTranslator* supports this standard-to-standard translation by organizing all metadata content into its own [internal metadata content standard](../mdtranslator/internalObject.md).  Each reader them must write its metadata content into *mdTranslator's* internal data store so that any of the writers can read and write from this store.  

The following sections will describe the *mdTranslator* in greater detail.

[__Installation__](../mdtranslator/installation.md) - covers installing the mdTranslator in Ruby, Ruby on Rails, coding environments.

[__Architecture__](../mdtranslator/architecture.md) - covers the mdTranslator architecture and the architectures of the command line interface (CLI) and the Ruby on Rails (RoR) interface. 

[__Usage__](../mdtranslator/usage.md) - covers accessing mdTranslator from Ruby code, the command line interface (CLI), and Ruby on Rails (RoR).

[__Extending the mdTranslator__](../mdtranslator/development.md) - covers extending mdTranslator by writing your own Reader or Writer. 
