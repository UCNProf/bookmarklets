---
title: UCN PWU Bookmarklet Collection
layout: default
---

Here you will find a collection of bookmarklets.
Most of them are only useful in the context of [UCN](https://ucn.dk).

<section class="bmls">
{% for bml in site.bookmarklets %}
<article class="bml" id="{{ bml.id | slugify}}">
  <header>
    <h3>{{ bml.title }}</h3>
  </header>
  <div class="bml-btn"><a href="{{ bml.script | escape_once | strip_newlines }}">{{ bml.title }}</a></div>
  <div class="bml-content">
    {{ bml.content | markdownify}}
  </div>
</article>
{% endfor %}
</section>

## How to use a bookmarklet

A bookmarklet is "installed" in your browser by adding it to your favorites.

1. Either right-click on the bookmarklet and select "Bookmark Link" or drag the bookmarklet to you bookmarks toolbar.
2. Open a website and click the bookmarklet in your favorites/bokmarks toolbar.