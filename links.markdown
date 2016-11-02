---
layout: page
title: Links
permalink: /links/
---

<ul>
	{% for link in site.data.links %}
	<li>
		<a href="{{ link.url }}">{{ link.text }}</a>
		<p>{{ link.desc }}</p>
	</li>
	{% endfor %}
</ul>
