---
layout: page
permalink: /publications/
title: publications
description:
years:
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<div markdown="1">
This is a list:

- Item 1
- Item 2
- Item 3
</div>
