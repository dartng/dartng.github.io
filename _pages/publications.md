---
layout: page
permalink: /publications/
title: publications
description: published work in journals and conferences
years: [2021, 2020, 2022]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
