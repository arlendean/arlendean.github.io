---
layout: page
permalink: /Research/
title: Research
description:
years:
nav: true
nav_order: 1
years: [2022]
---


<div class="post">
  <article>
    <div class="cvtwo">
      {% for entry in site.data.publications %}
        <div class="cardtwo mt-3 p-1">
        <h3 class="card-title font-weight-bold">{{ entry.title }}</h3>
          <div>
          {% if entry.type == "list" %}
            {% include cv/list.html %}
          {% elsif entry.type == "map" %}
            {% include cv/map.html %}
          {% elsif entry.type == "nested_list" %}
            {% include cv/nested_list.html %}
          {% elsif entry.type == "time_table" %}
           {% include cv/time_table.html %}
          {% else %}
            {{ entry.contents }}
          {% endif %}
          </div>
        </div>
      {% endfor %}
      </div>
  </article>
</div>

---

<div class="post">
    <div class="cvtwo">
      {% for entry in site.data.submittedpapers %}
        <div class="cardtwo mt-3 p-1">
          <h3 class="card-title font-weight-bold">{{ entry.title }}</h3>
          <div>
          {% if entry.type == "list" %}
            {% include cv/list.html %}
          {% elsif entry.type == "map" %}
            {% include cv/map.html %}
          {% elsif entry.type == "nested_list" %}
            {% include cv/nested_list.html %}
          {% elsif entry.type == "time_table" %}
           {% include cv/time_table.html %}
          {% else %}
            {{ entry.contents }}
          {% endif %}
          </div>
        </div>
      {% endfor %}
      </div>
</div>

---

<div class="post">
    <div class="cvtwo">
      {% for entry in site.data.workingpapers %}
        <div class="cardtwo mt-3 p-1">
          <h3 class="card-title font-weight-bold">{{ entry.title }}</h3>
          <div>
          {% if entry.type == "list" %}
            {% include cv/list.html %}
          {% elsif entry.type == "map" %}
            {% include cv/map.html %}
          {% elsif entry.type == "nested_list" %}
            {% include cv/nested_list.html %}
          {% elsif entry.type == "time_table" %}
           {% include cv/time_table.html %}
          {% else %}
            {{ entry.contents }}
          {% endif %}
          </div>
        </div>
      {% endfor %}
      </div>
</div>
