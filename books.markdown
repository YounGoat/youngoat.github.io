---
layout: page
title: Books
permalink: /books/
---

<ul>
	{% for book in site.data.books %}
	<li>
		<p>
			{% if book.local %}<a href="/books/{{ book.local }}">{% endif %}
			<em>{{ book.title_en }}</em>
			<br/>
			{{ book.title_cn }}
			{% if book.local %}</a>{% endif %}
			<br/>
			<small>
				<a href="{{ book.gitbook }}">@GitBook</a>
			</small>
		</p>
	</li>
	{% endfor %}
</ul>

<small>
See my profile at GitBook for more books:  
[https://www.gitbook.com/@youngoat](https://www.gitbook.com/@youngoat)
</small>
