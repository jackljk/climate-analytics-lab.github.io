---
title: " "
layout: posts
permalink: /projects/
entries_layout: grid
classes: wide

header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/podcast-header.png
  caption: "Photo credit: [**Third Pod from the Sun**](https://thirdpodfromthesun.com/)"


# https://mmistakes.github.io/minimal-mistakes/portfolio/
---

# Projects

Samples of published and ongoing projects by CCOG. Sort them by computational or Earth Science tags.\
Exciting new CCOG focus areas include sea level and large scale climate dynamics.

{% case site.tag_archive.type %}
  {% when "liquid" %}
    {% assign path_type = "#" %}
  {% when "jekyll-archives" %}
    {% assign path_type = nil %}
{% endcase %}

<p class="page__taxonomy">
  <span itemprop="keywords">
  {% for tag in site.tags %}
    <a href="{{  tag[0] | slugify | prepend: path_type | prepend: site.tag_archive.path | relative_url }}" class="page__taxonomy-item p-category" rel="tag">{{ tag[0] }}</a>{% unless forloop.last %}<span class="sep">, </span>{% endunless %}
  {% endfor %}
  </span>
</p>

<!-- Coming soon! -->