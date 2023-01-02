---
layout: default
title: Bookmarks
permalink: /bookmarks/
---
<h2>LouD - links to my sites / socials</h2>
<ul>
    <li>
        <a href="">{{ site.data.bookmarks.loud.description }}</a>
        ({{ site.data.bookmarks.loud.links | size }} bookmarks)
    </li>
</ul>

<h2>Bookmarks</h2>
<ul>
{% for bookmark in site.data.bookmarks %}
    {% assign name = bookmark[0] %}
    {% assign content = bookmark[1] %}
        {% if name != 'loud' %}
            <li>
                <a href="{{ '/bookmarks/'}}{{ content.permalink }}">{{ content.description }}</a>
                ({{ content.links | size }} bookmarks)
            </li>
        {% endif %}
{% endfor %}
</ul>
