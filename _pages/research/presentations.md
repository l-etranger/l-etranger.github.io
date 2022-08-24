---
layout: custom/page
permalink: /research/presentations/
title: presentations
description: presentations by categories in reversed chronological order
years_defenses: [2019]
years_conferences: [2019]
years_workshops: [2017]
years_seminars: [2022, 2020, 2019, 2017]
years_popularizations: [2018]
nav: false
---
<!-- _pages/presentations.md -->

<div class="publications">
<h1>defences</h1>
{%- for y in page.years_defenses %}
  {% bibliography -f defenses -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>conferences</h1>
{%- for y in page.years_conferences %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>workshops</h1>
{%- for y in page.years_workshops %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshops -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>seminars</h1>
{%- for y in page.years_seminars %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f seminars -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>popularizations</h1>
{%- for y in page.years_popularizations %}
  {% bibliography -f popularizations -q @*[year={{y}}]* %}
{% endfor %}
</div>