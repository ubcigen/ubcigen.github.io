---
layout: page
title: "Presidents Updates"
permalink: /news/presidents-updates/
---

<div class="container">



		{% for post in site.categories.president-update %}
  	{% assign loopindex = forloop.index | modulo: 2 %}
  	{% if loopindex == 1 %}
    <div class ="col-md-4">
      <div class ="thumbnail">
        <a href="{{ post.url }}"><h4>{{ post.title }}</h4></a>
        <p>{{ post.date | date_to_string }} &middot; {{ post.author }}</p>
      </div>
    </div>    
  	{% else %}
    <div class="col-md-4">
      <div class="thumbnail">
        <a href="{{ post.url }}"><h4>{{ post.title }}</h4></a>
        <p>{{ post.date | date_to_string }} &middot; {{ post.author }}</p>
      </div>  
    </div>
  	{% endif %}
		{% endfor %}




</div>
