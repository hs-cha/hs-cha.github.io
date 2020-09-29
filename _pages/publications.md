---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
# years: [1956, 1950, 1935, 1905]
# years: [2020, 2019, 2018, 2017, 2016, 2015]
journal_years: [2020, 2019, 2018, 2017, 2016, 2015]
submitted_years: [2020]
nav: true
---

<header class="post-header">
    <h1 class="post-title">Published</h1>
    <p class="post-description">Ten papers were published in SCI journals and one was published in a non-SCI journal</p>
</header>


<div class="publications">

{% for y in page.journal_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


<header class="post-header">
    <h1 class="post-title"><br/><br/>Submitted</h1>
    <p class="post-description">Two papers were under review and one was under preparation.</p>
</header>


<div class="publications">

<!-- {% for y in page.submitted_years %} -->
  <!-- <h2 class="year">{{y}}</h2> -->
  {% bibliography -f submitted%}
<!-- {% endfor %} -->

</div>

<!-- <header class="post-header">
    <h1 class="post-title"><br/><br/> International Conferences</h1>
    <p class="post-description">{{ page.description }}</p>
</header>


<div class="publications">

{% for y in page.conference_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>  -->