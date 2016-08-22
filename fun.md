---
layout: page
title: Fun
permalink: /fun/
---

{% for post in site.categories.fun %}

#<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

##<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

{% endfor %}