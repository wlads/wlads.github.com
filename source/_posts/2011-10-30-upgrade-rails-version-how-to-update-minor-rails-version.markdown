---
layout: post
title: "Upgrade rails version: how to update minor rails version"
date: 2011-10-30 14:37
comments: true
categories: [rails, version, update, upgrade]
---
This post shows how simple is to update one minor version from *Rails 3.1.0* to *Rails 3.1.1*, of course to update major versions like 2.X to 3.X you have a lot of trouble and tutorials available, also to upgrade from Rails 3.0.X to Rails 3.1.X you have a new feature called Asset Pipeline.

This is the Gemfile spec for rails 3.1.0
``` ruby 
gem 'rails', '3.1.0'

group :assets do
  gem 'sass-rails', "  ~> 3.1.0"
  gem 'coffee-rails', "~> 3.1.0"
  gem 'uglifier'
end
```
This is the Gemfile spec for rails 3.1.1
``` ruby
gem 'rails', '3.1.1'

group :assets do
  gem 'sass-rails',   '~> 3.1.4'
  gem 'coffee-rails', '~> 3.1.1'
  gem 'uglifier', '>= 1.0.3'
end
```