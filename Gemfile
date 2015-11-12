source 'https://rubygems.org'

ruby '2.2.3'

gem 'pg'
gem 'active_model_serializers'
gem 'rack-timeout'
gem 'rails', '4.2.2'
gem 'sass-rails', '~> 5.0'
gem 'responders', '~> 2.0'
gem 'unicorn'

group :development do
  gem 'spring'
  gem 'spring-commands-rspec'
end

group :development, :test do
  gem 'bundler-audit', require: false
  gem 'byebug'
  gem 'pry-rails'
  gem 'dotenv-rails'
  gem 'factory_girl_rails'
  gem 'rspec-rails', '~> 3.1.0'
  gem 'rubocop'
  gem 'rails_best_practices'
end

group :test do
  gem 'database_cleaner'
  gem 'shoulda-matchers', require: false
  gem 'webmock'
  gem 'simplecov', require: false
  gem 'mocha'
end
