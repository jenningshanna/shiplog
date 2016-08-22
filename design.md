---
layout: page
title: Design
permalink: /design/
---

{% for post in site.categories.design %}

<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

{% endfor %}