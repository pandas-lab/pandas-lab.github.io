---
layout: page
title: Categories
permalink: /categories/
---

<div>
{% for post in site.authors %}
  {% capture role_name %}{{ post.title | first }}{% endcapture %}
  <div class="archive-group">
    <h1>{{ role_name }}</h1>
    <h1>HERE</h1>
  </div>
{% endfor %}
</div>

<div>
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>
    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>

