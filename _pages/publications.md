---
layout: page
permalink: /publications/
title: publications
description:
years: [2023, 2022, 2021, 2020]
nav: true
nav_order: 1
---
For an updated list of publications, please see <a href='https://scholar.google.com/citations?user=ZNsw8ZUAAAAJ&hl=es'>Google Scholar</a>.

[\*]() Equal contribution
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
