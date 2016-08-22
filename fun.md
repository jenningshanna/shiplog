---
layout: page
title: Fun
permalink: /fun/
---

{% for post in site.categories.fun %}

<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

{% endfor %}