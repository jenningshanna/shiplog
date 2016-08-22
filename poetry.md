---
layout: page
title: Poetry
permalink: /poetry/
---

{% for post in site.categories.poetry %}

#<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

##<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

{% endfor %}