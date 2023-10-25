---
layout: default
---

<center><h2>About</h2></center>

{% for agegroup in site.soccer %}

<div class="wrap-collabsible"> <input id="collapsible{{-agegroup.maxage-}}" class="toggle" type="checkbox"> <label for="collapsible{{-agegroup.maxage-}}" class="lbl-toggle">


<!---###################################################--->
<!---TITLE OF GROUP GOES HERE>>>>--->U{{- agegroup.maxage -}}
<!---###################################################--->


</label><div class="collapsible-content"><div class="content-inner">

<!--- See the file yearsborn.html in the _includes folder for the specific phrasing of this part--->


{% include yearsborn.html %}


{{ agegroup.content }}

<a href="{{ site.data.navigation.soccer.fee }}"><div class="contentInnerButton">
<br>Register - Fee {{agegroup.fee}}<br><br>
</div></a>

</div></div></div>


{% endfor %}
