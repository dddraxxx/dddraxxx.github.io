---
layout: page
permalink: /publications/
title: Publications
description: <b>The authors with * contributed equally to the work</b>
nav: false
nav_order: 1
years: [2025, 2023, 2022]
---
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[writing_year={{y}}]* %}
{% endfor %}

</div>
