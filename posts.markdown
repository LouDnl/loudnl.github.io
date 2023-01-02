---
layout: default
title: Posts
permalink: /posts/
---
<h1>All Articles</h1>
<ul>
    {% for post in site.posts%}
        <li>
        <a href="{{ post.url }}">{{ post.title }}</a><br>
        <small>By {{ post.author }} on {{ post.date | date: "%-d %B %Y" }}</small>
        </li>
    {% endfor %}
</ul>
