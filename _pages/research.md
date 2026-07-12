---
layout: page
permalink: /Research/
title: Research
description:
nav: true
nav_order: 1
---

{% assign paper_groups = site.data.publications | concat: site.data.submittedpapers | concat: site.data.workingpapers %}

<div class="papers">
{% for entry in paper_groups %}
  <section class="paper-section">
    <h2 class="section-heading">{{ entry.title }}</h2>
    <ul class="paper-list">
      {% for paper in entry.contents %}
      <li class="paper">
        <h3 class="paper-title">{{ paper.title }}</h3>
        {% if paper.institution %}
        <p class="paper-authors">{{ paper.institution }}</p>
        {% endif %}
        {% if paper.description %}
        <ul class="paper-notes">
          {% for note in paper.description %}
          <li>{{ note }}</li>
          {% endfor %}
        </ul>
        {% endif %}
      </li>
      {% endfor %}
    </ul>
  </section>
{% endfor %}
</div>
