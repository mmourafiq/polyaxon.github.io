bundle install
copy generated `site` from polyaxon to `\docs`
bundle exec jekyll build
bundle exec jekyll serve --watch
JEKYLL_ENV=production bundle exec rake site:publish
