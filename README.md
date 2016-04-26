# Directory Structure and Files in the Root Directory

* `404.html` - contains jekyll variables and options
* `_config.yml` - contains jekyll variables and options
* `_includes/` - reusable chunks of html (`{% include foo.html %}`)
* `_layouts/` - reusable markup (jekyll layouts) used by including metadata at the top of file:
```
---
layout: default
---
```
* `_posts/` - .md or .html files containing the a post's content
* `_sass/` - .scss files containing the css for the site
* `_sass/` - .scss files containing the css for the site
* `public/` - a directory containing public assets (currently images/icons/fonts)
* `tag/` - a directory that contains the .html index files for each 'tag' on the site (ie. big-data, tips-and-tricks)



# Jekyll Info

[Jekyll Documentation](https://jekyllrb.com/)

## Running Jekyll Locally

```bash
jekyll serve --watch`
```

```bash
jekyll serve --watch --drafts`
```

