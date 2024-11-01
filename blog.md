---
layout: default
title: Blog
---

# Blog

<ul>
  {% for post in site.categories.blog %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%B %d, %Y" }}</time>
    </li>
  {% endfor %}
</ul>
