---
title: "Gut Intelligence Lab - Team"
layout: gridlay
excerpt: "Gut Intelligence Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

<!-- ## Team -->
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i> <br>
  <!-- <br>email: <{{ member.email }}> -->
  <p class='social'> 
  {% if member.email != null %}  <a href="mailto:{{ member.email }}">  <i class="fa fa-envelope" aria-hidden="true"></i></a>  {% endif %}  {% if member.github != null %}  <a href="{{ member.github }}"><i class="fa fa-github" aria-hidden="true"></i></a>  {% endif %} {% if member.linkedin != null %}  <a href="{{ member.linkedin }}"><i class="fa fa-linkedin" aria-hidden="true"></i></a>  {% endif %} {% if member.scholar != null %}  <a href="{{ member.scholar }}"><i class="ai ai-google-scholar-square" aria-hidden="true"></i></a>  {% endif %} {% if member.rg != null %}  <a href="{{ member.rg }}"><i class="ai ai-researchgate" aria-hidden="true"></i></a>  {% endif %} 
  </p>
  
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}



<!-- ## Master and Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %} -->

#### Click here for [Alumni]({{ site.baseurl }}/alumni) and [Collaborators]({{ site.baseurl }}/collaborators)

### Administrative Contact

{% assign number_printed = 0 %}
{% for member in site.data.admin %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i> <br>
  <!-- <br>email: <{{ member.email }}> -->
  <p class='social'> 
  {% if member.email != null %}  <a href="mailto:{{ member.email }}">  <i class="fa fa-globe" aria-hidden="true"></i></a>  {% endif %}  {% if member.github != null %}  <a href="{{ member.github }}"><i class="fa fa-github" aria-hidden="true"></i></a>  {% endif %} {% if member.linkedin != null %}  <a href="{{ member.linkedin }}"><i class="fa fa-linkedin" aria-hidden="true"></i></a>  {% endif %} {% if member.scholar != null %}  <a href="{{ member.scholar }}"><i class="ai ai-google-scholar-square" aria-hidden="true"></i></a>  {% endif %} 
  </p>
  
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

### Be a part of the future of AI in gastroenterology!
![fun_team_pic]({{ site.baseurl }}/images/chrcdsiteam.jpg){:class="img-responsive"}

<button style="padding: 10px 10px; font-size: 15px; border-radius: 10px;" type="button" class="btn btn-primary" onclick=" relocate_home()">Come Work With Us!</button>

(We also offer short 1-2 month electives for students interested in learning more about what we do.)