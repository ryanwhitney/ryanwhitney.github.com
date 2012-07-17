---
layout: page
title: Ryan Whitney - Design & Development
---
{% include JB/setup %}


<ul class="posts">
{% for post in site.posts %}
	<a href="http://ryan.whitney.me"><nav class="link left">Portfolio</nav></a>

	<li>
		<h2>
			{% if  post.src %}
				<a class="linked" href="{{ BASE_PATH }}{{ post.src }}">{{ post.title }}</a>
			{% else %}
				<a class="local" href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
			{% endif %}
		</h2>
		<span class="date">{{ post.date | date: " %B %d, %Y" }}</span>
		{{ post.content }}
		<hr class="seperator">
	</li>
{% endfor %}
</ul>
