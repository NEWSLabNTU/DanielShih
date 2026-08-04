source 'https://rubygems.org'

# Jekyll 4.3 — built and deployed with GitHub Actions (not the github-pages gem,
# which pins Jekyll 3.9 and forbids the custom plugin in _plugins/).
gem 'jekyll', '~> 4.3.4'

group :jekyll_plugins do
  gem 'jekyll-email-protect', '~> 1.1'
  gem 'jekyll-paginate', '~> 1.1'
  gem 'jekyll-scholar', '~> 7.1'
  gem 'jemoji', '~> 0.13'
end

# kramdown 2.x ships the GFM parser separately; needed for `input: GFM`.
gem 'kramdown-parser-gfm', '~> 1.1'

# Ruby 3.x no longer bundles a web server for `jekyll serve`.
gem 'webrick', '~> 1.8'

# Gems unbundled from the Ruby stdlib in 3.4, still required by transitive deps.
gem 'base64', '~> 0.2'
gem 'bigdecimal', '~> 3.1'
gem 'csv', '~> 3.3'
gem 'logger', '~> 1.6'
gem 'ostruct', '~> 0.6'

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem 'tzinfo', '>= 1', '< 3'
  gem 'tzinfo-data'
end
