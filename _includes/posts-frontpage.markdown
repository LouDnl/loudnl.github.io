<h1>Latest Article</h1>

{{ site.posts.first.content | strip_html | truncatewords:75}}  \
<a href="{{ site.posts.first.url }}">Continue reading: {{ site.posts.first.title }}</a>

<h1>Recent Articles</h1>
{% include index_post_list.html %}
