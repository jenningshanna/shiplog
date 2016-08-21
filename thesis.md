---
layout: page
title: SVA IxD Thesis
permalink: /thesis/
---

{% for post in site.categories.thesis %}

#<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

##<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

{% endfor %}