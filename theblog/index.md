---
layout: blog
title: "PayPad: blog"
---

<div>

	{% for post in site.posts %}
		<article>
			<p class="date">{{ post.date | date: "%B %e, %Y" }}</p>
			<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
			{{ post.excerpt | markdownify }} <a href="{{ post.url }}" class="continue">read more...</a>
		</article>
	{% endfor %}

</div>