---
layout: page
title: Project Showcase
permalink: /industry/project-showcase/
---

<div class="container">

<p>This annual event showcases innovative and multidisciplinary engineering design projects. The event is a great opportunity to learn about this exciting program, network with students and faculty members, and see some of the projects this year's student groups have put together, as well as the solutions to this year's IGEN Challenges.</p>

<h2>Attend the Project Showcase</h2>

RSVP to attend this year's event. Click the button below.<br>
<a class ="btn btn-primary" href="http://engineering.ubc.ca/event/2016/integrated-engineering-project-showcase" target="_blank" role="button">RSVP</a>
<br><br>
<hr>

<p>For more information about the IGEN Project Showcase please email industry@integratedengineers.ca, and to view past projects from previous years follow the link below.</p>

<a href="/industry/current-projects">See this year's projects</a>

<br><br>

        {% for post in site.posts %}
          {% if page.categories =="IGEN-Project" %}
          <li>
            <a href="{{ post.url }}">{{ post.title }}</a>
          </li>
          {% endif %}

        {% endfor %}


</div>
