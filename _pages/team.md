---
#layout: archive
title: "Team"
permalink: /team/
author_profile: true
---

**We are looking for new PhD students, research assistants, and visitors to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**

## PhD Students

<div class="team-section">
  {% assign number_printed = 0 %}
  {% for member in site.data.team_stu %}

    {% assign even_odd = number_printed | modulo: 2 %}

    {% if even_odd == 0 %}
    <div class="row">
    {% endif %}

    <div class="col-sm-6 clearfix" style="margin-bottom: 20px;">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="15%" style="float: left; margin-right: 15px; border-radius: 5px;" />
      <h4 style="font-size: 1.2em; font-weight: bold; margin-top: 0;">{{ member.name }}</h4>
      <i style="display: block; font-size: 0.95em; margin-bottom: 10px;">{{ member.info }}</i>
      <ul style="overflow: hidden; margin: 0; padding-left: 1em; list-style-type: disc;"> 
        {% if member.number_educ >= 1 %}
        <li>{{ member.education1 }}</li>
        {% endif %}
        {% if member.number_educ >= 2 %}
        <li>{{ member.education2 }}</li>
        {% endif %}
        {% if member.number_educ == 3 %}
        <li>{{ member.education3 }}</li>
        {% endif %}
      </ul>
    </div>

    {% assign number_printed = number_printed | plus: 1 %}

    {% if even_odd == 1 %}
    </div> <!-- Close row after two members -->
    {% endif %}

  {% endfor %}

  {% assign even_odd = number_printed | modulo: 2 %}
  {% if even_odd == 1 %}
  </div> <!-- Close row if the last row has an odd number of members -->
  {% endif %}
</div> <!-- End of team-section -->






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


 
