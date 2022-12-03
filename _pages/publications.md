---
layout: page
permalink: /Publications/
title: Publications
description: publications by categories in reversed chronological order. 
years: [2012,2011,2010]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
