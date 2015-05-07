---
layout: page
title: Members
excerpt: "The MINED Group @ Georgia Tech"
search_omit: false
---

<ul class="post-list">
	{% for post in site.posts %} 
		{% if post.categories contains 'members' %}
			<li>
				<article>
					<a href="{{ site.url }}{{ post.url }}">{{ post.author.name }} <span class="entry-date">Updated: <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.author.role %} <span class="excerpt">{{ post.role }}</span>{% endif %}</a>
				</article>
			</li>
		{% endif %}
	{% endfor %}
</ul>
