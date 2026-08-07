source "https://rubygems.org"

gem "jekyll", "~> 4.3"

# The `github-pages` meta-gem pins very old exact versions to mirror GitHub's
# production build, which regularly fails to compile native extensions on modern
# Ruby. Instead we install the individual plugins this theme's _config.yml and
# includes actually reference, matching what GitHub Pages' whitelist provides.
group :jekyll_plugins do
  gem "jekyll-include-cache",        "~> 0.2"   # {% include_cached %} tag used throughout
  gem "jekyll-optional-front-matter","~> 0.3"   # lets pages skip the --- --- front matter
  gem "jekyll-titles-from-headings", "~> 0.5"   # derives page titles from first heading
  gem "jekyll-relative-links",       "~> 0.6"   # rewrites relative links to .md files
  gem "jekyll-seo-tag",              "~> 2.8"
  gem "jekyll-feed",                 "~> 0.17"
  gem "jekyll-avatar",               "~> 0.8"
end

# Ruby 3+ no longer bundles webrick, but `jekyll serve` needs it.
gem "webrick", "~> 1.8"
