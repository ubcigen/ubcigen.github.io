---
layout: page
title: News
permalink: /news/
---

<div class="container">
	
	{% for post in site.posts %}
  {% assign loopindex = forloop.index | modulo: 2 %}
  {% if loopindex == 1 %}
    <div>
      <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
      <p>{{ post.date | date_to_string }} | {{post.author}}</p>
  {% else %}
      <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
      <p>{{ post.date | date_to_string }} | {{post.author}}</p>
    </div>
  {% endif %}
{% endfor %}	
	
</div>