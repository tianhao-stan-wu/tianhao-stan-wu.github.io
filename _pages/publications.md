---
layout: page
permalink: /publications/
title: publications
description: Working hard to publish some papers...
years: [1, 2, 3]
nav: true
nav_order: 2
---
<!-- years: [add years here; e.g 2022, 2023, ...] -->

<!-- _pages/publications.md -->
<div class="publications">


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
