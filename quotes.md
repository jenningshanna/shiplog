---
layout: page
title: Quotes
permalink: /quotes/
---

{% for post in site.categories.quotes %}

#<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

##<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

{% endfor %}