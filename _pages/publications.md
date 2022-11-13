---
layout: page
permalink: /publications/
title: publications
# description: This page only shows selected publications. The full publication list is available on <a href='https://scholar.google.com/citations?user=C8M7-1YAAAAJ'>google scholar</a>.
years: [2022, 2019]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
