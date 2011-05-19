---
title: Community
layout: default
kicker: Community - Blog
message: The Jentrata community is here to help
current-cm: current_page_item
---
<ul class="unordered">
{% for post in site.posts %}
{% if post.category != 'sidebar' then %}
	<li><a href="{{ post.url }}">{{ post.title }}</a> - <abbr>{{ post.date | date_to_string }}</abbr></li>
{% endif %}
{% endfor %}
</ul>