# mdTranslator

### Configuration Files

__travis.yml__ is the Travis CI (Continuous Integration) configuration file.  It specifies the versions of Ruby to test mdTranslator against. 

![Travis CI File](/assets/mdTranslator/travis.png){caption}
````ruby

sudo: false
language: ruby
before_install: 'gem install bundler'
rvm:
  - "2.4"
  - "2.5"
  - "2.6"
  - jruby-head
  - ruby-head
matrix:
  allow_failures:
    - rvm: jruby-head

````

__adiwg-mdtranslator.gemspec__ lists the dependent Ruby GEMs for mdTranslator.  The Gem's version is also managed from this file. 

![Gemspec File](/assets/mdTranslator/gemspec.png){caption}

__rakefile__ controls which tests are run from the terminal with the "rake" command.  Notice each reader and writer is listed on a separate line so one or more can be easily isolated during frequent testing periods or when changes are made to the mdJson schema which effect multiple readers and writers.  

![Gemspec File](/assets/mdTranslator/rakefile.png){caption}
