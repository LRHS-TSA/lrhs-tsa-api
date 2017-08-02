source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end


## Core

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 5.0.2'
# Use sqlite3 as the database for Active Record
gem 'sqlite3'
# Use Puma as the app server
gem 'puma', '~> 3.7.1'
# Use MySQL2 for production database
gem 'mysql2'
# Use Redis adapter to run Action Cable in production
gem 'redis', '~> 3.0'

## Assets

# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.6.3'
# bundle exec rake doc:rails generates the API under doc/api.
gem 'sdoc', '~> 1.0.0.rc2', group: :doc

## Models

# Validate email format without Regex
gem 'validates_email_format_of'
# Validate phone number format
gem 'phony_rails'
# Use ActiveModel has_secure_password
gem 'bcrypt', '~> 3.1.11'

## Controllers and Application Logic

# Use respond_to in controller and respond_with
gem 'responders', '~> 2.3.0'
# Use devise for authentication
gem 'devise', '~> 4.2.1'
# Add token authentication to devise
gem 'devise_token_auth', '~> 0.1.42'
# Provide authorization using CanCanCan
gem 'cancancan', '~> 1.16.0'
# Use Delayed Job as a jobs backend
gem 'delayed_job', '~> 4.1.2'
# Use ActiveRecord with Delayed Job
gem 'delayed_job_active_record', '~> 4.1.1'



group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platform: :mri
end


group :development do
  ## Debugging

  # View emails in dev environments
  gem 'letter_opener', '~> 1.4.1'

  ## Refactoring

  # Use rubocop to check style
  gem 'rubocop', '~> 0.48.1', require: false
  # Check style for tests
  gem 'rubocop-rspec', require: false
  # Use bullet to find performace issues
  gem 'bullet', '~> 5.5.1'
  # Lock down the formatting of schema.rb
  gem 'fix-db-schema-conflicts', '~> 2.0.0'

  ## Security

  # Audit the gemfile for insecure gems
  gem 'bundler-audit', '~> 0.5.0', require: false
  # Scan the application for vulnerabilities
  gem 'brakeman', '~> 3.6.1', require: false

  ## Utilitly

  # Watches the filesystem for changes
  gem 'listen', '~> 3.1.5'
  # Keep the application loaded in the background
  gem 'spring', '~> 2.0.1'
  # Update spring using listen
  gem 'spring-watcher-listen', '~> 2.0.1'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
