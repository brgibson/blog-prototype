---
layout: post
title: Getting Started with Jekyll
tags: [Front End, github, github-pages, jekyll]
summary: Here are the most helpful links for understanding the open source Jekyll blogging framework.  This new blogging framework has built in integration with github pages and is great for generating static sites.
image: http://4.bp.blogspot.com/-1ApahgMBJVE/Vba02LAZwRI/AAAAAAAACMc/JpUx0KKrvVE/s1600/Screen%2BShot%2B2015-07-27%2Bat%2B3.42.44%2BPM.png
---

Ben, again.  Here are the most helpful links for understanding how Jekyll works once it's up and running.

- [Jekyll Structure](http://jekyllrb.com/docs/structure/)
- http://jekyllrb.com/docs/pages/#homepage

The homepage uses a regular template like everything else...

<iframe width="560" height="315" src="https://www.youtube.com/embed/oDQZu8K51ZY" frameborder="0" allowfullscreen></iframe>

_index.html_
{% highlight html %}

---
layout: default
title: Home
---

<div class="posts">
  { % for post in paginator.posts %} <!-- I put in a space between the { and % so this would work... -->
  <article class="post">
    <h1 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

    ...
{% endhighlight %}

- http://jekyllrb.com/docs/posts/#displaying-an-index-of-posts
- http://jekyllrb.com/docs/posts/#post-excerpts
- http://jekyllrb.com/docs/templates/#code-snippet-highlighting
- https://demisx.github.io/jekyll/2014/01/13/improve-code-highlighting-in-jekyll.html
- http://jekyllrb.com/docs/templates/

In a template file (ie. any file?) the _&#123;&#123; content }}_ variable comes from the content of the file that says layout, your specific template... (if that makes sense)

- http://jekyllrb.com/docs/configuration/#front-matter-defaults
- http://jekyllrb.com/docs/frontmatter/
- http://www.minddust.com/post/tags-and-categories-on-github-pages/
- http://www.geligalabs.com/code/2014/06/19/jekyll-category-list.html
- https://github.com/Shopify/liquid/wiki/Liquid-for-Designers - jekyll function reference

