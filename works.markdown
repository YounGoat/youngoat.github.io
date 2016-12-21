---
layout: page
title: Works
permalink: /works/
---

### Books

<ul>
	{% for book in site.data.books %}
	<li>
		<p>
			<em>{{ book.title_en }}</em>
			<br/>
			{{ book.title_cn }}
			<br/>
			<small>
				<a href="{{ book.gitbook }}">@GitBook</a>
				{% if book.local %}
					&nbsp;<a href="/books/{{ book.local }}">Read</a>
				{% endif %}
			</small>
		</p>
	</li>
	{% endfor %}
</ul>


### Node.js Products

*   *yuan*  
    <small>Collection of syntax sugar for JavaScript</small>

*   *yuan-console*  
    <small>NodeJS SDK for CLI development</small>
