---
layout: page
permalink: /publications/
title: publications
description:
years: [1956, 1950, 1935, 1905]
nav: true
---

<div markdown="1">
   **peer-reviewed journal articles**
</div>

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers2 -q @*[year={{y}}]* %}
{% endfor %}

</div>

<div markdown="1">
   **peer-reviewed conference papers**
</div>

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
