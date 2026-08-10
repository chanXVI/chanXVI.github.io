# sanilBlog

Jekyll blog boilerplate for a GitHub Pages site.

## Current status

This repo is using the default Jekyll scaffold with the `minima` theme:

- `_config.yml` contains the site settings and enables `jekyll-feed`
- `index.markdown` uses the default home layout
- `about.markdown` is the starter About page
- `_posts/` contains the starter welcome post
- `.github/workflows/jekyll-gh-pages.yml` builds and deploys the site with GitHub Pages Actions

The generated `_site/` output and local Bundler files are ignored by Git.

## Local development

Install the Ruby gems:

```bash
bundle install
```

Run the local Jekyll server:

```bash
bundle exec jekyll serve
```

For automatic browser refresh while editing posts, pages, or styles, run:

```bash
bundle exec jekyll serve --livereload
```

Optional shell shortcut for `~/.zshrc`:

```zsh
alias js='bundle exec jekyll serve --livereload'
```

After adding the alias, reload your shell config:

```bash
source ~/.zshrc
```

Then run the shortcut from this project directory:

```bash
js
```

Then open the local URL printed by Jekyll, usually:

```text
http://127.0.0.1:4000/
```

## Deployment

Push changes to `main`. The GitHub Actions workflow builds the Jekyll site and deploys the generated artifact to GitHub Pages.
