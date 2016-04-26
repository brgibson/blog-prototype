# Directory Structure and Files in the Root Directory

* <pre>404.html</pre> - contains jekyll variables and options
* <pre>_config.yml</pre> - contains jekyll variables and options
* <pre>_includes/</pre> - reusable chunks of html (<pre>{% include foo.html %}</pre>)
* <pre>_layouts/</pre> - reusable markup (jekyll layouts) used by including metadata at the top of file:
    ---
    layout: default
    ---
* <pre>_posts/</pre> - .md or .html files containing the a post's content
* <pre>_sass/</pre> - .scss files containing the css for the site
* <pre>_sass/</pre> - .scss files containing the css for the site
* <pre>public/</pre> - a directory containing public assets (currently images/icons/fonts)
* <pre>tag/</pre> - a directory that contains the .html index files for each 'tag' on the site (ie. big-data, tips-and-tricks)



# Jekyll Info

[Jekyll Documentation](https://jekyllrb.com/)

## Running Jekyll Locally

$ jekyll serve --watch
$ jekyll serve --watch --drafts

