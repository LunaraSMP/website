---
layout: blog
title: Blog
---

<div class="blog-content">
    <h1>Blog</h1>
    <p>Welcome to our blog! Here you will find updates, announcements, and community stories.</p>
    <ul>
        {% for post in site.posts %}
            <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                <span>{{ post.date | date: '%B %d, %Y' }}</span>
            </li>
        {% endfor %}
    </ul>
</div>