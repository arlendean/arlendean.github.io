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
### Publications
<div class="post">
  <article>
    <div class="cvtwo">
      {% for entry in site.data.publications %}
        <div class="cardtwo mt-3 p-1">
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
    <div class="cvtwo">
      {% for entry in site.data.submittedpapers %}
        <div class="cardtwo mt-3 p-1">
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
      <div class="cvtwo">
        <div class="cardtwo mt-3 p-1">
      {% for entry in site.data.workingpapers %}
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

      {% endfor %}
              </div>
              </div>
</div>


---
