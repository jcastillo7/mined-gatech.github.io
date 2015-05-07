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
					{% if post.author.image %}<img src="{{ post.author.image }}" style="float: left; height: 75px; border-radius: 50%; padding-right: 50px">{% endif %}
					<a href="{{ site.url }}{{ post.url }}">{{ post.author.name }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.author.role %} <span class="excerpt">{{ post.author.role }}</span>{% endif %}</a>
				</article>
			</li>
		{% endif %}
	{% endfor %}
</ul>
