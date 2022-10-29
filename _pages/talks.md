---
layout: page
permalink: /talks/
title: talks
description: talks by categories in reversed chronological order. generated by jekyll-scholar.
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>