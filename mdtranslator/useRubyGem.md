#mdTranslator

## Installation

### Ruby

Installation of the 'adiwg-mdtranslator' RubyGem is discussed in the section [Installation in Ruby](../mdtranslator/installInRuby.md).  After installation, the 'adiwg-mdtranlator' gem is access through a single exposed method - 'translate'. 

Example call to translate:
````ruby
metadata = ADIWG::Mdtranslator.translate(
    file: jsonObj, reader: 'mdJson', validate: 'normal',
    writer: 'iso19115_2', showAllTags: true)
````

The translate method uses a named parameter list so the order of parameters is not important. The translate method takes the following parameters:

__file:__ - 