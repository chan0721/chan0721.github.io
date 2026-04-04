---
layout: page
title: 数学学习
permalink: /physics/
---

<h1>数学学习</h1>

<ul>
  {% for post in site.categories.physics %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span> - {{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>
