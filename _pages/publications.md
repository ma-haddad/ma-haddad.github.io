---
layout: page
permalink: /Publications/
title: Publications
description: <b> Under construction -> To be completed soon!</b>
years: [2026,2025,2024,2023,2022,2021,2020,2019,2016,2015,2014,2013,2012,2011]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->

<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{ y }}]* %}
{% endfor %}

</div>
