---
layout: page
permalink: /publications/
title: publications
description: <h5>You can find my peer-reviewed publications below or on my <a href = 'https://scholar.google.com/citations?user=9B1Rs6sAAAAJ&hl=en'>Google Scholar page</a>.</h5>
years: [2024,2023,2022,2020]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
