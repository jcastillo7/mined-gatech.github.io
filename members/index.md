---
layout: page
title: Members
excerpt: "The MINED Group @ Georgia Tech"
search_omit: false
---

<ul class="post-list">
	{% for post in site.categories.members %} 
	<li>
		<article>
			<a href="{{ site.url }}{{ post.url }}">{{ post.name }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.role %} <span class="excerpt">{{ post.role }}</span>{% endif %}</a>
		</article>
	</li>
	{% endfor %}
</ul>
