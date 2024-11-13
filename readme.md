# Jekyll Installation and Usage Guide

1. Install Jekyll and Bundler gems:
   ```bash
   gem install jekyll bundler
   ```

2. Update your Gemfile with required dependencies:
   ```ruby
   gem "jekyll"
   ```

3. Install dependencies:
   ```bash
   bundle install
   ```

## Building Your Site

Jekyll needs to build the site before you can view it. Use one of these commands:

* `jekyll build`: Builds the site and outputs to `_site` directory
* `jekyll serve`: Builds and serves the site at `http://localhost:4000`, auto-rebuilding on changes

To ensure you're using the correct versions, prefix commands with `bundle exec`: