---
layout: default
title: baseball
---

<center><h2>About</h2></center>

{% for agegroup in site.baseball %}

<div class="wrap-collabsible"> <input id="collapsible{{-agegroup.maxage-}}" class="toggle" type="checkbox"> <label for="collapsible{{-agegroup.maxage-}}" class="lbl-toggle">


<!---###################################################--->
<!---TITLE OF GROUP GOES HERE>>>>--->U{{- agegroup.maxage -}}
<!---###################################################--->


</label><div class="collapsible-content"><div class="content-inner">

<!--- See the file yearsborn.html in the _includes folder for the specific phrasing of this part--->

<h1>{{ agegroup.title }}</h1>

{% include yearsborn.html %}


{{ agegroup.content }}

{% if agegroup.maxage != 17 %}

<a href="
{% for item in site.data.navigation %}
{% if item.name == "Baseball" %}
{{item.register}}
{% endif %}
{% endfor %}
"><div class="contentInnerButton">
<br>Register - Fee {{agegroup.fee}}<br><br>
</div></a>

{% endif %}

</div></div></div>

{% endfor %}
