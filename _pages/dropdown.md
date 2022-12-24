---
layout: page
permalink: /Talks/
title: Talks
years: [2021,2022,2023]
nav: true
nav_order: 2
---
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<!--
<div class="post">
  {%- include talks.html %}
</div> -->
