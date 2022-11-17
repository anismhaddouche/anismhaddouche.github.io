---
layout: page
permalink: /Talks/
title: Talks
description: 
years: [2018,2020,2021,2022]
nav: true
nav_order: 3
---
<!-- _pages/talks.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>


