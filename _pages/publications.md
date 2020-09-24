---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
# years: [1956, 1950, 1935, 1905]
years: [2020, 2020, 2019, 2018, 2017, 2017, 2017, 2016, 2016, 2016, 2015]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
