source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

ruby '2.3.1'
gem 'rails', '~> 5.0.1'

# Datastore
gem 'pg', '~> 0.18'
gem 'redis', '~> 3.0'

# App server
gem 'puma', '~> 3.0'

# Core
gem 'bcrypt', '~> 3.1.7'

# AAA
gem 'pundit'

# View
gem 'sass-rails', '~> 5.0'
gem 'uglifier', '>= 1.3.0'
gem 'coffee-rails', '~> 4.2'
gem 'jquery-rails'
gem 'turbolinks', '~> 5'

# API
gem 'jbuilder', '~> 2.5'

group :development do
  gem 'web-console', '>= 3.3.0'
  gem 'listen', '~> 3.0.5'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
  
  # SCA
  gem 'rubocop'
  gem 'reek'
  gem 'brakeman'
end

group :development, :test do
  # Tooling
  gem 'pry-rails'
  gem 'pry-byebug'

  # Debugging
  gem 'byebug', platform: :mri

  # Testing frameworks
  gem 'rspec-rails', '~> 3.5.0'
  gem 'fuubar'
  gem 'factory_girl_rails'
  gem 'faker'
end

group :test do
  # Coverage
  gem 'coveralls', require: false

  # Testing frameworks
  gem 'capybara'
  gem 'shoulda-matchers', '~> 3.1'
end
