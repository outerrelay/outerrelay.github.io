---
layout: default
title: Home
---
<section class="hero">
  <p class="eyebrow">Research-based analysis</p>
  <h1 class="home-title">Economic security, trade dependencies, and strategic resilience.</h1>
  <p class="lead">This blog is a space for evidence-based writing on trade dependencies, reverse dependencies, energy security, and related topics. Posts are designed to be transparent about methods, data sources, and limitations.</p>
  <div class="hero-actions">
    <a class="button-primary" href="{{ '/about/' | relative_url }}">About the blog</a>
    <a class="button-secondary" href="{{ '/categories/' | relative_url }}">Browse categories</a>
  </div>
</section>

<section class="grid-two">
  <div class="card">
    <h2>What you can expect</h2>
    <ul class="plain-list">
      <li>Short research notes and longer analytical essays</li>
      <li>Replication of public methodologies where possible</li>
      <li>Clear sourcing, data notes, and measured claims</li>
      <li>A focus on Norway in comparative European context</li>
    </ul>
  </div>
  <div class="card accent-card">
    <h2>Core themes</h2>
    <p>Trade dependencies, reverse dependencies, energy security, critical supply chains, economic statecraft, and strategic exposure.</p>
  </div>
</section>

<section class="section-block">
  <div class="section-heading">
    <h2>Recent posts</h2>
    <a href="{{ '/categories/' | relative_url }}">View all categories</a>
  </div>

  {% assign recent_posts = site.posts | slice: 0, 6 %}
  {% if recent_posts.size > 0 %}
    <div class="post-list">
      {% for post in recent_posts %}
        <article class="post-card">
          <p class="small-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
          <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
          {% if post.excerpt %}<p>{{ post.excerpt }}</p>{% endif %}
          <div class="tag-row">
            {% for category in post.categories %}
              <a class="tag" href="{{ '/category/' | append: category | append: '/' | relative_url }}">{{ category | replace: '-', ' ' }}</a>
            {% endfor %}
          </div>
        </article>
      {% endfor %}
    </div>
  {% else %}
    <div class="card">
      <p>No posts yet. Add your first post in the <code>_posts</code> folder.</p>
    </div>
  {% endif %}
</section>
