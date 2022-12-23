---
layout: page
permalink: /publications/
title: Research
description:
years: [2021, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
 My research has primarily focused on improving patient care quality through addressing various hospital operations problems.
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
