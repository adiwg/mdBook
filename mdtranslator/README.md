# mdTranslator

## Overview
The *mdTranslator* is the heart of the ISO Metadata Developer's Toolkit. The *mdTranslator* translates metadata content from any supported reader format into any of the supported writer formats.  The *mdTranslator* supports this standard-to-standard translation by organizing all metadata content into its own [internal metadata content standard](../mdtranslator/internalObject.md).  Each reader them must write its metadata content into *mdTranslator's* internal data store so that any of the writers can read and write from this store.  

The following sections will describe the *mdTranslator* in greater detail.

[__Installation__](../mdtranslator/installation.md) - 

[__Architecture__](../mdtranslator/architecture.md) - 

[__Usage__](../mdtranslator/usage.md) - 

[__Extending the mdTranslator__](../mdtranslator/development.md) - 