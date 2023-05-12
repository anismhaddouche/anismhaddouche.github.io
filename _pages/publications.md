---
layout: page
permalink: /publications/
title: Publications
description: All my published papers in reverse chronological order.
years: [2018,2020,2021,2022,2023]
nav: true
nav_order: 1
---
<!-- _pages/talks.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


