---
layout: page
permalink: /publications/
title: publications
description: My Publications
years: [2024]
nav: True
nav_order: 7
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
