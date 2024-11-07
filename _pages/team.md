---
permalink: /
title: "Team"
excerpt: "Team"
author_profile: true
redirect_from: 
  - /team/
  - /team.html
---


# Group Members

**We are  looking for new PhD students, research assistants, and visitors to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!** 


## PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.team_students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1}} </li>
  <li> {{ member.education2}} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
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


<!-- ## Alumni
<div class="row">

<div class="col-sm-4 clearfix">
<h4>Staff</h4>
{% for member in site.data.alumni_staff %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Students</h4>
{% for member in site.data.alumni_student %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Visitors</h4>
{% for member in site.data.alumni_visitor %}
{{ member.name }}
{% endfor %}
</div>

</div> -->


 
