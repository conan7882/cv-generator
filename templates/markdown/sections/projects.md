{% extends "section.md" %}

{% block body %}
<table class="table table-hover">
{% for r in items %}
<tr>
<td class="col-md-3"><a><img src='{{ r.im }}'  onerror="this.onerror=null;this.src='images/projects/alt.jpg';"/></a> </td>
<td>
    <strong>{{ r.name }}</strong><br>
    {{ r.details_short }}<br>
    {{ r.details_list }}
    {{ r.links }}
    {{ r.details }}
</td>
</tr>
{% endfor %}
</table>

{% endblock body %}
