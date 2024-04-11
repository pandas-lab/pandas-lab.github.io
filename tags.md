---
layout: page
title: Research Areas
featured-img: bamboo-09.jpeg
permalink: /tags/
---

<div>
{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
  <div class="archive-group">
    {% capture tag_name %}{{ tag | first }}{% endcapture %}
    <div id="#{{ tag_name | slugize }}"></div>
    <p></p>
    <h3 class="category-head">{{ tag_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.tags[tag_name] %}
    <article class="archive-item">
      <a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>

