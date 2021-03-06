source 'https://rubygems.org'

puppet_version = ENV['PUPPET_GEM_VERSION']

gem 'puppet', (puppet_version.nil? ? '~> 6.0' : puppet_version)

group :development do
  gem 'codacy-coverage', '2.1.0'
  gem 'coderay', '1.1.2'
  gem 'mdl', '0.5.0'
  gem 'metadata-json-lint', '2.2.0'
  gem 'pdk', '1.13.0'
  gem 'puppetlabs_spec_helper', '2.14.1'
  gem 'rake', '13.0.0'
  gem 'rspec-puppet-facts', '1.9.5'
  gem 'semantic_puppet' if puppet_version.to_f < 4.9
  gem 'simplecov', '0.17.1'
end

group :acceptance_testing do
  gem 'beaker', '4.13.0'
  gem 'beaker-puppet', '1.18.8'
  gem 'beaker-rspec', '6.2.4'
  gem 'beaker-vagrant', '0.6.2'
end

group :documentation do
  gem 'puppet-strings', '2.3.1'
  gem 'redcarpet', '3.5.0'
end

group :release do
  gem 'github_api', '0.18.2'
  gem 'puppet-blacksmith', '5.0.0'
end

group :metatools do
  gem 'github-linguist', '7.6.1'
  gem 'overcommit', '0.51.0'
  gem 'rubocop', '0.75.0'
  gem 'rubocop-performance', '1.5.0'
  gem 'rubocop-rspec', '1.36.0'
  gem 'travis', '1.8.10'
end
