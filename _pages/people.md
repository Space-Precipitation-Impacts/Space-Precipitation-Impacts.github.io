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


<div class="display compact" style="height:100%; width:130%; font-size:	12px; overflow:auto;">

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

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.10.13/js/jquery.dataTables.min.js"></script>

<script type="text/javascript"
        src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>

<script>
 
$(document).ready(function() {
    $("#catalogue").dataTable( {
        paging: false,
        'data-sort': true,
        order: [[ 0, "desc" ], [3, "desc"]],
        stateSave: true,
        searching: true
    });
});
</script>