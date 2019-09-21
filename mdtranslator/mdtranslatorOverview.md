# mdTranslator
[![Build Status](https://travis-ci.org/adiwg/mdTranslator.svg?branch=master)](https://travis-ci.org/adiwg/mdTranslator)
[![Gem Version](https://badge.fury.io/rb/adiwg-mdtranslator.svg)](http://badge.fury.io/rb/adiwg-mdtranslator)

## Overview
**mdTranslator** is the engine of the mdToolkit. It translates metadata content in any supported reader format into any of the supported writer formats.  mdTranslator supports this standard-to-standard translation by organizing all metadata content into its own [internal metadata content standard](extend/internalObject.md).  Each mdTranslator reader must write its metadata content into the internal data store so that any of the writers can then read and write from this store.

The following sections will describe the mdTranslator in greater detail and include instructions for coding new readers and writers.

[__Installation__](install/installation.md) - covers installing the mdTranslator in Ruby, Ruby on Rails, coding environments.

[__Architecture__](architecture/architecture.md) - covers the mdTranslator architecture and the architectures of the command line interface (CLI) and the Ruby on Rails (RoR) interface.

[__Usage__](use/usage.md) - covers accessing mdTranslator from Ruby code, the command line interface (CLI), and Ruby on Rails (RoR).

[__Extending the mdTranslator__](extend/extendTranslator.md) - covers extending mdTranslator by writing your own reader or writer.
