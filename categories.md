---
title: Categories
lead: "A structured overview of the blog's main themes."
permalink: /categories/
---

<div class="category-grid">
  {% assign category_names = site.category_descriptions | map: "first" %}
  {% for item in site.category_descriptions %}
    {% assign category_name = item[0] %}
    {% assign category_description = item[1] %}
    {% assign category_posts = site.categories[category_name] %}
    <article class="card">
      <h2><a href="{{ '/category/' | append: category_name | append: '/' | relative_url }}">{{ category_name | replace: '-', ' ' }}</a></h2>
      <p>{{ category_description }}</p>
      <p class="small-meta">{{ category_posts | size }} post{% if category_posts.size != 1 %}s{% endif %}</p>
    </article>
  {% endfor %}
</div>
