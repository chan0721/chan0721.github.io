---
layout: page
title: 随笔
permalink: /journal/
---

<h1>随笔</h1>

<ul>
  {% for post in site.tags.journal %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span> - {{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>
