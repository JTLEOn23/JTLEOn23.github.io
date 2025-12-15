source "https://rubygems.org"

# Jekyll
gem "jekyll", "~> 4.4.1"

# Theme Minimal Mistakes no necesita estar en el Gemfile si usamos 'remote_theme'
# en _config.yml, pero incluimos los plugins necesarios.

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-sitemap"
  gem "jekyll-include-cache"
end

# Windows and JRuby platforms
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]