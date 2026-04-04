---
layout: page
title: 数学学习
permalink: /physics/
---

<div class="post-list">
  {% for post in site.tags.math %}
    <div class="post-list-item">
      <h2 class="post-list-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h2>
      <p class="post-list-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
      </p>
      {% if post.excerpt %}
        <div class="post-list-excerpt">
          {{ post.excerpt }}
        </div>
      {% endif %}
    </div>
  {% endfor %}
</div>
