---
title: Community
layout: default
kicker: Community - Blog
message: The Jentrata community is here to help
current-cm: current_page_item
---

{% for post in site.categories.blog limit:10 %}

 <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
 
 <div class="posted">Posted by <span class="author">{{ post.author }}</span> on {{ post.date | date_to_string }}</div>

{{ post.content | truncate:40 }}</p>
 <!-- this is due to a bug with Jekyll. Truncate truncates a p tag. -->
 <a href="{{ post.url }}" title="Continue Reading">Continue Reading &raquo;</a>
-------------
	


{% endfor %}

