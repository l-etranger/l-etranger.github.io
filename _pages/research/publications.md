---
layout: custom/page
permalink: /research/publications/
title: publications
description: publications by categories in reversed chronological order
years_thesis: [2019]
years_preprints: [2022]
years_publications: [2022, 2019, 2018, 2017]
years_internships: [2016, 2015, 2014, 2013]
years_contributions: [2021]
nav: false
---
<!-- _pages/publications.md -->

<div class="publications">
<h1>thesis</h1>
{%- for y in page.years_thesis %}
  {% bibliography -f thesis -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>preprints</h1>
{%- for y in page.years_preprints %}
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>publications</h1>
{%- for y in page.years_publications %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f publications -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>internships</h1>
{%- for y in page.years_internships %}
  {% bibliography -f internships -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h1>contributions</h1>
{%- for y in page.years_contributions %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f contributions -q @*[year={{y}}]* %}
{% endfor %}
</div>