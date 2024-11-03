---
layout: default
title: Blog
---

<header>
    <nav>
        <ul>
            <li><a href="{{ site.baseurl }}/">Home</a></li>
            <li><a href="{{ site.baseurl }}/about/">About</a></li>
            <li><a href="{{ site.baseurl }}/blog/">Blog</a></li>
            <li><a href="{{ site.baseurl }}/community/">Community</a></li>
            <li><a href="{{ site.baseurl }}/support/">Support</a></li>
            <li><a href="{{ site.baseurl }}/store/">Store</a></li>
        </ul>
    </nav>
</header>
<h1>Blog</h1>
<p>Welcome to the Blog page! Here you can find our latest posts and updates.</p>

<ul>
    {% for post in site.posts %}
        <li>
            <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
        </li>
    {% endfor %}
</ul>

<footer>
    <p>© 2024 {{ site.author }}. All rights reserved.</p>
    <p>Website designed with help from ChatGPT.</p>
</footer>
