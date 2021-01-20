---
layout: page
permalink: /publications/
title: publications
description: selected publications
a-years: [2021, 2019, 2018, 2013, 2012]
p-years: [2020, 2017, 2016, 2012]
t-years: [2020, 2013, 2011]
m-years: [2021, 2015, 2014, 2010, 2009]
nav: true
---

## peer-reviewed journal articles

<div class="publications">

{% for y in page.a-years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f articles -q @*[year={{y}}]* %}
{% endfor %}

</div>

___

<br>

## peer-reviewed conference papers

<div class="publications">

{% for y in page.p-years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers2 -q @*[year={{y}}]* %}
{% endfor %}

</div>

___

<br>

## theses

<div class="publications">

{% for y in page.t-years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f theses -q @*[year={{y}}]* %}
{% endfor %}

</div>

<br>

## music 

<div class="publications">

{% for y in page.m-years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f music -q @*[year={{y}}]* %}
{% endfor %}

</div>

