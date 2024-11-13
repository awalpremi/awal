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



rename blog posts properly otherwise they dont show up. 
mv _posts/blog1.md _posts/2023-10-12-blog1.md

make a bunch of blog posts with ai content like this or in python
for i in {1..5}; do
  touch "$(date +%Y-%m-%d)-post$i.md"
done


this makes sure the correct front matter is in there.
cd _posts
for i in {1..5}; do
  filename="$(date +%Y-%m-%d)-post$i.md"
  cat <<EOL > "$filename"
---
layout: post
author: murph
title: Post $i
---
Content for Post $i goes here.
EOL
done