---
layout: page
permalink: /publications/
title: publications
description: academic publications troughtout my life 
years: [2018, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
