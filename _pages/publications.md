---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

<div class="publications">
  <h1>Journal Papers</h1>
  {% bibliography -f papers %}

  <h1>Conference Proceedings</h1>
  {% for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {% bibliography -f proceedings -q @*[year={{y}}]* %}
  {% endfor %}

  </div>
