---
layout: page
permalink: /Research/
title: Research
description:
years:
nav: true
nav_order: 1
years: [2021,2022,2023]
---
### Publications
<div class="post">
  <article>
    <div class="cv">
      {% for entry in site.data.publications %}
        <div class="card mt-3 p-1">
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

### Submitted Papers

<div class="post">
    <div class="cv">
      {% for entry in site.data.submittedpapers %}
        <div class="card mt-3 p-1">
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

### Working Papers

<div class="post">
    <div class="cv">
      {% for entry in site.data.workingpapers %}
        <div class="card mt-3 p-1">
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

### Trial

<div class="post">
    <div class="cv">
      {% for entry in site.data.workingpapers %}
        <div class="card mt-3 p-1">
          <div>
          {% if entry.type == "list" %}
            {% include cv/list.html %}
          {% elsif entry.type == "map" %}
            {% include cv/map.html %}
          {% elsif entry.type == "nested_list" %}
            {% include cv/nested_list.html %}
          {% elsif entry.type == "time_table" %}
          <div class="publications">
          {%- for y in page.years %}
            <h2 class="year">{{y}}</h2>
            {% bibliography -f papers -q @*[year={{y}}]* %}
          {% endfor %}

          </div>
          {% else %}
            {{ entry.contents }}
          {% endif %}
          </div>
        </div>
      {% endfor %}
      </div>
</div>
