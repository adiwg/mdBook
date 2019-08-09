# mdTranslator

## Configuration Files

### Rake

__Rakefile__ controls which tests are run from the terminal with the "rake" command.  Notice each reader and writer is listed on a separate line so one or more can be easily isolated during frequent testing periods or when changes are made to the mdJson schema which effect multiple readers and writers.  

````ruby

require 'bundler/gem_tasks'
require 'rake/testtask'

Rake::TestTask.new do |t|
   t.libs << 'test'
   t.test_files = FileList[
      'test/readers/fgdc/tc*.rb',
      'test/readers/mdJson/tc*.rb',
      'test/readers/sbJson/tc*.rb',
      'test/writers/fgdc/tc*.rb',
      'test/writers/html/tc*.rb',
      'test/writers/iso19110/tc*.rb',
      'test/writers/iso19115-1/tc*.rb',
      'test/writers/iso19115-2/tc*.rb',
      'test/writers/mdJson/tc*.rb',
      'test/writers/sbJson/tc*.rb',
      'test/translator/tc*.rb'
   ]
   t.verbose = true
end

desc 'Run tests'
task :default => :test

````
### Travis

__travis.yml__ is the Travis CI (Continuous Integration) configuration file.  It specifies the versions of Ruby to test mdTranslator against. 

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
