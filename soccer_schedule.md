---
layout: default
---

<div class="contentLeft">

{% for agegroup in site.soccer %}

<h3> U{{- agegroup.maxage }} </h3>

<p>{{ agegroup.time }}</p>

<p>Home games and practices at {{ agegroup.location }}</p>

{% endfor %}

</div>


{% include soccerlocations.html %}
