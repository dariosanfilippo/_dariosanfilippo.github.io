---
layout: page
permalink: /publications/
title: publications
description:
a-years: [2020, 2019, 2018, 2013, 2012]
p-years: [2017, 2016, 2012]
t-years: [2020, 2013]
nav: true
---

#### peer-reviewed journal articles

<div class="publications">

{% for y in page.a-years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f articles -q @*[year={{y}}]* %}
{% endfor %}

</div>

___

#### peer-reviewed conference papers

<div class="publications">

{% for y in page.p-years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers2 -q @*[year={{y}}]* %}
{% endfor %}

</div>

___

#### theses

<div class="publications">

{% for y in page.t-years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f theses -q @*[year={{y}}]* %}
{% endfor %}

</div>

