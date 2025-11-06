# frozen_string_literal: true

source "https://rubygems.org"

gem "json"

gemspec

gem "html-proofer", "~> 5.0", group: :test

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-include-cache"
end

gem "wdm", "~> 0.2.0", :platforms => [:mingw, :x64_mingw, :mswin]


gem "jekyll"
gem "jekyll-paginate"
gem "jekyll-archives"
gem "jekyll-seo-tag"
gem "jekyll-gist"
gem "jemoji"
gem "jekyll-sitemap"