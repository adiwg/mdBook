# mdTranslator

## RubyGem dependencies

mdTranslator has the following dependent RubyGems:

````ruby

   spec.required_ruby_version = '>= 2.3'

   spec.add_development_dependency "bundler", "~> 2"
   spec.add_development_dependency "rake", "~> 10"
   spec.add_development_dependency "minitest", "~> 5"

   spec.add_runtime_dependency "json", "~> 2.0"
   spec.add_runtime_dependency "builder", "~> 3.2"
   spec.add_runtime_dependency "thor", "~> 0.19"
   spec.add_runtime_dependency "uuidtools", "~> 2.1"
   spec.add_runtime_dependency "json-schema", "~> 2.7"
   spec.add_runtime_dependency "adiwg-mdjson_schemas", ">= 2.6"
   spec.add_runtime_dependency "adiwg-mdcodes", "~> 2.7"
   spec.add_runtime_dependency "jbuilder", "~> 2.5"
   spec.add_runtime_dependency "kramdown", "~> 1.13"
   spec.add_runtime_dependency "coderay", "~> 1.1"
   spec.add_runtime_dependency "nokogiri", "~> 1.7"

````

These will automatically install with the adiwg-mdtranslator gem if they are not already installed.
