gem install jekyll bundler
update gemfile to have what you need like gem "jekyll"
install everything by running bundle


Since Jekyll is a static site generator, it has to build the site before we can view it. Run either of the following commands to build your site:

jekyll build - Builds the site and outputs a static site to a directory called _site.
jekyll serve - Does jekyll build and runs it on a local web server at http://localhost:4000, rebuilding the site any time you make a change.