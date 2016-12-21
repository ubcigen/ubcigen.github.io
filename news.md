---
title: News
permalink: "/news/"
layout: page
---

<div class="container">



		{% for post in site.posts %}
  	{% assign loopindex = forloop.index | modulo: 2 %}
  	{% if loopindex == 1 %}
    <div class ="col-md-4">
      <div class ="thumbnail">
        <a href="{{ post.url }}"><h4>{{ post.title }}</h4></a>
        <p>{{ post.date | date_to_string }} &middot; {{post.categories}}</p>
        <img class="img-responsive" src="{{ post.image }}">
      </div>
    </div>    
  	{% else %}
    <div class="col-md-4">
      <div class="thumbnail">
        <a href="{{ post.url }}"><h4>{{ post.title }}</h4></a>
        <p>{{ post.date | date_to_string }} &middot; {{post.categories}}</p>
        <img class="img-responsive" src="{{ post.image }}">
      </div>  
    </div>
  	{% endif %}
		{% endfor %}




</div>
