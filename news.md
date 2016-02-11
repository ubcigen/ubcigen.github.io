---
layout: page
title: News
permalink: /news/
---

<div class="container">



		{% for post in site.posts %}
  	{% assign loopindex = forloop.index | modulo: 2 %}
  	{% if loopindex == 1 %}
    <div class ="col-md-4">
      <div class ="thumbnail">
        <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
        <p>{{ post.date | date_to_string }} &middot; {{post.categories}} &middot; {{post.author}}</p>
        <img class="img-responsive" src="{{ post.image }}">
      </div>
    </div>    
  	{% else %}
    <div class="col-md-4">
      <div class="thumbnail">
        <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
        <p>{{ post.date | date_to_string }} &middot; {{post.categories}} &middot; {{post.author}}</p>
        <img class="img-responsive" src="{{ post.image }}">
      </div>  
    </div>
  	{% endif %}
		{% endfor %}




</div>
