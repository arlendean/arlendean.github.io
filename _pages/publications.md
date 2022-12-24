---
layout: page
permalink: /publications/
title: Research
description:
years:
nav: true
nav_order: 1
---
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

**Publications:**

1. Quantile Regression Forests for Individualized Surgery Scheduling

    Dean, A., Meisami, A., Lam, H., Van Oyen, M., Stromblad, C., Kastango, N

   - Health care Management Science, 2022



**Papers Under Revision:**

Dean, A., Zhaelchian, M., Van Oyen, M. “Dynamic Care Unit Placements under Unknown Demand with Learning.” Major Revision MSOM.


**Working Papers:**

Zhaelchian, M., Fu, D.J., Dean, A., Van Oyen, M., Stein, J., Khawaja, A., Lavieri, M.“Forecasting Visual-field Loss in Open-angle Glaucoma Patients by Application of Kalman-filtering to 20 Years of Real-World, Multicenter Data.” Preparing for submission.

Dean, A., Zhaelchian, M., Garifullin, M., Pardo, J., Van Oyen, M. “Real-time Matching of Patients to Beds in Hospital Systems: Implementation and Theory.” Working paper.

Dean, A., Zhaelchian, M., Shi, C.“Online Learning and Pricing in Multi-Reusable Resource Settings.” Working paper.
