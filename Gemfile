# frozen_string_literal: true

source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/digitalocean/hacktoberfest.git" }

gem 'airbrake', '~> 9.4'
gem 'airrecord'

gem 'bootsnap', '>= 1.1.0', require: false
gem 'bulma-rails', '~> 0.7.5'

gem 'coffee-rails', '~> 5.0', '>= 5.0.0'

gem 'dalli', '~> 2.7'

gem 'faraday'
gem 'faraday_middleware'

gem 'health_check', '>= 3.1.0'

gem 'jbuilder', '~> 2.10', '>= 2.10.0'

gem 'kramdown'

gem 'loofah', '>= 2.4.0'

# Must be locked before version 3.0 for use with airrecord gems
# See: https://github.com/sirupsen/airrecord/issues/63
gem 'net-http-persistent', '~> 2.9'

gem 'octokit', '~> 4.19.0'
gem 'omniauth-github', '~> 2.0.0'
gem 'omniauth-rails_csrf_protection', '~> 1.0', '>= 1.0.0'

gem 'puma', '~> 4.0'

gem 'country_select', '~> 4.0', require: 'country_select_without_sort_alphabetical'

gem 'rails', '~> 7.1.0'

gem 'sass-rails', '~> 6.0', '>= 6.0.0'
gem 'sidekiq', '>= 5.2.9', '< 6.0'
gem 'sidekiq-scheduler', '>= 3.1.0'

gem 'figaro'

# commenting out these settings since we are not using enterprise sidekiq in local docker dev
#unless ENV['RAILS_ENV'] == 'production' || ENV['RAILS_ENV'] == 'staging' || ENV['REDIS_HOST'] == 'redis'
#  require 'dotenv'
#  Dotenv.load['BUNDLE_ENTERPRISE__CONTRIBSYS__COM']
#end

#install_if -> { ENV['BUNDLE_ENTERPRISE__CONTRIBSYS__COM'] } do
#  source 'https://enterprise.contribsys.com/' do
#    gem 'sidekiq-pro'
#    gem 'sidekiq-ent'
#  end
#end


gem 'state_machines'
gem 'state_machines-activerecord', '>= 0.8.0'

gem 'pg'
gem 'pry'

gem 'turbolinks', '~> 5'
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

gem 'uglifier', '>= 1.3.0'

group :development, :test do
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]

  gem 'dotenv-rails', '>= 2.7.6'

  gem 'factory_bot_rails', '>= 5.1.0'

  gem 'rspec-rails', '>= 3.8.3'
  gem 'rubocop-rails', '>= 2.4.0'

  gem 'shoulda-matchers', '>= 4.2.0'

  gem 'vcr'

  gem 'webmock'
end

group :development do
  gem 'capistrano', '~> 3.11', require: false
  gem 'capistrano-bundler', '~> 1.6', require: false
  gem 'capistrano-dotenv', require: false
  gem 'capistrano-rails', '~> 1.4', require: false
  gem 'capistrano3-puma', '~> 5.0', '>= 5.0.0', require: false
  gem 'capistrano-sidekiq', '>= 2.0.0', require: false

  gem 'guard-rspec', require: false

  gem 'listen', '>= 3.0.5', '< 3.2'

  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'

  gem 'terminal-notifier-guard'

  gem 'web-console', '>= 4.0.0'
end
