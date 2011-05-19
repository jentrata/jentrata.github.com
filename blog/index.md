---
title: Community
layout: default
kicker: Community - Blog
message: The Jentrata community is here to help
current-cm: current_page_item
---
<ul class="unordered">
{% for post in site.categories.blog %}
	<li><a href="{{ post.url }}">{{ post.title }}</a> - <abbr>{{ post.date | date_to_string }}</abbr></li>
{% endfor %}
</ul>