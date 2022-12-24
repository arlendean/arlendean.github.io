---
layout: page
permalink: /Talks/
title: Talks
description:  Abstracts for talks I have given.
nav: true
nav_order: 2
---

<div class="talks">
  <h3>INFORMS Annual Confernence</h3>
  {% if site.talks != blank -%}
  {%- assign talks_size = site.talks | size -%}
  <div class="table-responsive" {% if site.talks_scrollable and talks_size > 3 %}style="max-height: 10vw"{% endif %}>
    <table class="table table-sm table-borderless">
    {%- assign talks = site.talks | reverse -%}
    {% if site.talks_limit %}
    {% assign talks_limit = site.talks_limit %}
    {% else %}
    {% assign talks_limit = talks_size %}
    {% endif %}
    {% for item in talks limit: talks_limit %}
      <tr>
        <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
        <td>
          {% if item.inline -%}
            {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
          {%- else -%}
            <a class="talks-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
          {%- endif %}
        </td>
      </tr>
    {%- endfor %}
    </table>
  </div>
{%- else -%}
  <p>No talks so far...</p>
{%- endif %}
</div>
