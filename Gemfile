# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) { |repo| "https://github.com/#{repo}.git" }

group :development do
  gem "rspec"
  gem "rdoc"
  gem "rake", "~> 13.0.0.pre.1"
  gem "rubocop", require: false
  gem "rubocop-performance", require: false
  gem "rubocop-rails", require: false


  gem "activerecord",   github: "rails/rails", branch: "master", ref: '015c393'
  # gem "ruby-plsql", github: "rsim/ruby-plsql", branch: "master"
  gem "ruby-plsql", github: "bjfish/ruby-plsql", branch: "truffleruby-ci"

  platforms :ruby do
   #gem "ruby-oci8",    github: "kubo/ruby-oci8"
    gem "ruby-oci8", git: 'https://github.com/bjfish/ruby-oci8.git', branch: 'truffleruby-ci'
    gem "byebug"
  end

  platforms :jruby do
    gem "pry"
    gem "pry-nav"
  end
end
