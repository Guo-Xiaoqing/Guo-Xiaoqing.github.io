---
#layout: archive
title: "Team"
permalink: /team/
author_profile: true
---

# Group Members

**We are looking for new PhD students, research assistants, and visitors to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**

## PhD Students

<div class="team-section">
  {% assign number_printed = 0 %}
  {% for member in site.data.team_stu %}

    {% assign even_odd = number_printed | modulo: 2 %}

    {% if even_odd == 0 %}
    <div class="row">
    {% endif %}

    <div class="col-sm-6 clearfix">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
      <h4>{{ member.name }}</h4>
      <i>{{ member.info }}</i>
      <ul style="overflow: hidden"> 
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


 
