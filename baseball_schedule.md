---
layout: default
title: Baseball Schedule
---
{% for agegroup in site.baseball %}

<h3> U{{- agegroup.maxage }} </h3>
<h4> {{ agegroup.title }} </h4>

<p>{{ agegroup.time }}</p>

{% if agegroup.location %}

<p>Home games and practices at {{ agegroup.location }}</p>

{% endif %}

{% endfor %}
