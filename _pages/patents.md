---
layout: page
permalink: /patents/
title: patents
description: publications by categories in reversed chronological order
years: [2020, 2019, 2018, 2017, 2015]
nav: true
---


<header class="post-header">
    <h1 class="post-title">Patents</h1>
    <p class="post-description">Four patents were registered and six patentes were filed. Note that one was filed in USA</p>
</header>


<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f patents -q @*[year={{y}}]* %}
{% endfor %}

</div>