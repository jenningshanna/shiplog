---
layout: page
title: Poetry
permalink: /poetry/
---

{% for post in site.categories.poetry %}

<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

{% endfor %}