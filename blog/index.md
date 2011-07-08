---
title: Community
layout: default
kicker: Community - Blog
message: The Jentrata community is here to help
current-cm: current_page_item
---

{% for post in site.categories.blog limit:10 %}

{%if post.draft != 'true' %}

 <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
 
 <div class="posted">Posted by <span class="author">{{ post.author }}</span> on {{ post.date | date_to_string }} <a href="{{ post.url }}#disqus_thread">{{ post.title }}</a></div>

{{ post.content | strip_html | truncatewords:100 }}
 <a href="{{ post.url }}" title="Continue Reading">Continue Reading &raquo;</a>
-------------
{% endif %}
{% endfor %}

