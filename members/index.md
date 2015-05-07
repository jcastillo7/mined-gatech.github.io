---
layout: page
title: Members
excerpt: "The MINED Group @ Georgia Tech"
search_omit: false
---

<ul class="post-list">
	<table>
	{% for post in site.posts %} 
		{% if post.categories contains 'members' %}
		<tr>
		<td valign="middle">
			<li>
				{% if post.author.image %}<img src="{{ post.author.image }}" style="float: left; height: 125px; border-radius: 50%; border: 25px solid transparent">{% endif %}
					<article>					
						<a href="{{ site.url }}{{ post.url }}">{{ post.author.name }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.author.role %} <span class="excerpt">{{ post.author.role }}</span>{% endif %}</a>
					</article>
			</li>
		</td>
		</tr>
		{% endif %}
	{% endfor %}
</ul>
