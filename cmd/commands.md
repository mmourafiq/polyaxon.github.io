bundle install

copy generated `site` from polyaxon to `\docs`

```
cp -r path-to-polyaxon/docs/site/ docs/
git checkout -- docs/assets/images/favicon.ico
```

bundle exec jekyll build

bundle exec jekyll serve --watch

JEKYLL_ENV=production bundle exec rake site:publish
