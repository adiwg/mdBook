#mdTranslator

## Installation

### Ruby

Access to the mdTranslator after installation of the 'adiwg-mdtranslator' gem is through a call to single method.   
````ruby
# call mdtranslator with desired parameters
# mdtranslator uses a 'named' parameter list
metadata = ADIWG::Mdtranslator.translate(
    file: jsonObj, reader: 'mdJson', validate: 'normal',
    writer: 'iso19115_2', showAllTags: true)
````

