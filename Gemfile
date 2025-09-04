# Usa Ruby moderno para compatibilidad con sass-embedded
ruby "~> 3.3"          # acepta 3.3.0 … 3.3.x

source "https://rubygems.org"

# Núcleo Jekyll
gem "jekyll", "~> 4.4.1"

# Temas (puedes dejar solo el que uses)
gem "minima", "~> 2.5"
gem "jekyll-theme-merlot"
gem "jekyll-theme-cayman"
gem "jekyll-theme-modernist"
gem "jekyll-theme-primer"
gem "jekyll-theme-hacker"

# Plugins
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
end

# Soporte Windows/JRuby
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock para JRuby
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]


