---
layout: page
title: News
permalink: /news/
---

<div class="container">
	<ul>
	  {% for post in site.posts %}
	    <li>
	      <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
	    </li>
	    {{post.date.short}}
	    <div class="thumbnail">
	    	{{post.excerpt}}
	    </div>	
	  {% endfor %}
	</ul>
</div>