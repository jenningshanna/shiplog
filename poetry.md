---
layout: page
title: Poetry
permalink: /poetry/
---

{% for post in site.categories.poetry %}
    
<div class="post-list">
	    {% if post.image %}
	    	<a class="post-link post-image" href="{{ post.url | prepend: site.baseurl }}">
	      		<img src="{{ post.image | prepend: site.baseurl }}" alt="{{ post.title }}" title="{{ post.title }}">
      		</a>
	  	{% endif %}
<h2>
<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
</h2>
<img src="../images/dottedline.png" alt="dotted line" />
<em><small>{{ post.lead }}</small></em>
<br />
<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}&nbsp;</span>
</div>
      
{% endfor %}