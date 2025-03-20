---
layout: single
permalink: /publications/
title: Publications
description: 
years: [ 2024, 2022, 2021]
years_pre: [2025]
years_conference: [2024,2023, 2022, 2021, 2020, 2019]

nav: true
---


[[Google scholar](https://scholar.google.ca/citations?user=Jlnqt6MAAAAJ&hl=en)] | [[ORCID](https://orcid.org/0000-0003-4162-0073)] | [[View by Research Project](http://chenhbo.github.io/research/)]

&dagger;Equal Contribution.
#Co-Corresponding Author.

<hr style="border-top: 2px solid #ccc; margin: 20px 0;">


## Preprints

<div class="publications">

{% for y in page.years_pre %}
  <div style="font-size: 20px; font-style: italic;font-weight: bold;">-{{ y }}-</div>
  {% bibliography -f preprint -q @*[year={{y}}]* %}
  <hr style="border-top: 2px solid #ccc; margin: 20px 0;">

{% endfor %}

</div>



## Journals


<div class="publications">

{% for y in page.years %}
  <!-- <div style="font-size: 20px; font-style: italic;font-weight: bold;"><u>{{ y }}</u></div> -->
  <div style="font-size: 20px; font-style: italic;font-weight: bold;">-{{ y }}-</div>
  {% bibliography -f pubs -q @*[year={{y}}]* %}
  <hr style="border-top: 2px solid #ccc; margin: 20px 0;">

{% endfor %}

</div>


## Conferences



<div class="publications">


{% for y in page.years_conference %}
  <div style="font-size: 20px; font-style: italic;font-weight: bold;">-{{ y }}-</div>
  {% bibliography -f proceeding -q @*[year={{y}}]* %}
  <hr style="border-top: 2px solid #ccc; margin: 20px 0;">

{% endfor %}

</div>


