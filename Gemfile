source 'https://rubygems.org'

ruby '2.3.1'

gem 'dotenv-rails', :groups => [:development, :test]

gem 'rails', '~> 4.1'
gem 'rails-api'

# Database connection
gem 'activerecord-sqlserver-adapter', '4.1.2'
gem 'tiny_tds'

# JSON API
# Support the JSONAPI.org standard
gem 'jsonapi-resources',
  git: 'git://github.com/AKHarris/jsonapi-resources.git',
  ref: '05cbf3ed211fc9e048e01b7c14d5934df2558c2b'
gem 'versionist'

gem 'jsonapi-serializers' # Serialize with JSONAPI.org standard
gem 'kaminari'            # Pagination
gem 'api-pagination'      # Paginates API in headers
gem 'rack-cors', require: 'rack/cors' # CORS Headers
gem 'rmagick'             # Image processing
gem 'redis'               # Image caching

# Utilities
gem 'foreman'
gem 'wannabe_bool'        # Convert boolean-ish values to booleans
gem 'httparty'            # HTTP requests
gem 'rack-mini-profiler', require: false
gem 'flamegraph'
gem 'stackprof' # ruby 2.1+ only
gem 'memory_profiler'

group :development do
  gem 'byebug'
  gem 'spring'            # Keeps environment in background
  gem 'better_errors'     # Clearer error messages
  gem 'binding_of_caller' # Error message REPL & more
  gem 'rails-erd'         # Output data model diagrams
  gem 'yaml_db'
end

group :development, :test do
  gem 'pry-rails'
  gem 'pry-byebug'
  gem 'rspec-rails',        '~> 2.14.0' # Stick to a specific version
  gem 'spring-commands-rspec', '~> 1.0'
  gem 'factory_girl_rails',    '~> 4.0' # Build factories quickly
  gem 'database_cleaner'
  gem 'guard-rspec',            '4.3.1' # Autorun tests and keep Rails loaded
  gem 'faker'                           # Generate fake data
  gem 'vcr',                   '~> 2.4' # Record API calls for tests
  gem 'childprocess',          '~> 0.5' # Fix a version conflict
  gem 'webmock', '~> 1.8.4', require: false # Faking requests (supports VCR)
  gem 'minitest'
end

group :production do
  gem 'puma'           # App server
  gem 'rails_12factor' # Log output
  gem 'scout_apm'      # Memory leak hunter
end


gem 'pg' # For testing, and to get Heroku to deploy it.
