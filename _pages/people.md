---
layout: archive
permalink: /people/
title: "People"
excerpt: "Our Group"
author_profile: true
redirect_from: 
  - /people.html
---

{% assign file = site.data.personnel %}

# SPI Personnel


<div class="display compact" style="height:100%; width:75%; font-size:16px; overflow:auto;">

<table id="catalogue" class="display">
<thead>
<tr class="header">
<th style="font-size: 16px" data-sort>Personnel</th>
<th style="font-size: 16px">Institution</th>
<th style="font-size: 16px">Role</th>

</tr>
</thead>
<tbody>

{% for row in file %}
  <tr>
  <td> {{ row.Personnel }} </td>
  <td> {{ row.Institution }}</td>
  <td> {{ row.Role}} </td>
  </tr>
{% endfor %}
</tbody>
</table>

</div>
