# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# for old ruby 2.0.x (CentOS)
if RUBY_VERSION < "2.1"
  gem "public_suffix", "~> 2.0.5"
  gem "i18n", "~> 0.7.0"
  gem "rb-inotify", "~> 0.9.10"
  gem "listen", "~> 3.0.0"
  gem "jekyll-watch", "~> 1.4.0"
  gem "liquid", "~> 3.0.0"
end

gem "jekyll"
