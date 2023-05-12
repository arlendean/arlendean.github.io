---
layout: page
permalink: /Talks/
title: Talks
years: [2023,2022,2021]
nav: true
nav_order: 2
---
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>

<!--
<div class="post">
  {%- include talks.html %}
</div> -->
