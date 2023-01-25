---
layout: page
permalink: /publications/
title: Publications
description: <b>* denotes cofirst author</b>
nav: false
nav_order: 1
years: [2022]
---
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[writing_year={{y}}]* %}
{% endfor %}

</div>
