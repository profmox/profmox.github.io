source "https://rubygems.org"

# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!
gem "jekyll", "~> 4.4.1"

# This is the default theme for new Jekyll sites. You may change this to anything you like.
gem "minima", "~> 2.5"

# NOTE: github-pages gem is intentionally NOT used here — it pins Ruby < 4.0
# and we're on Ruby 4.0.3. GitHub Pages still builds the deployed site using
# its own pipeline regardless of this Gemfile.

# If you have any plugins, put them here!
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# NOTE: `wdm` (Windows file-watch booster) removed — does not compile on Ruby 4.
# Jekyll falls back to polling for --watch on Windows, which is fine for a small site.

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
