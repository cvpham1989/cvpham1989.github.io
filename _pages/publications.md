---
layout: page
permalink: /publications/
title: Publications
description: #
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="filter-buttons">
  <a href="/publications">All</a>
  <a href="/publications?type=article">Journal</a>
  <a href="/publications?type=inproceedings">Proceedings</a>
</div>
<div class="publications">
{% if paginator.page.param contains 'article' %}

  {% bibliography -f {{site.scholar.bibliography}} --query @*[type=article] %}

{% elsif paginator.page.param contains 'inproceedings' %}

  {% bibliography -f {{site.scholar.bibliography}} --query @*[type=inproceedings] %}

{% else %}

  {% bibliography -f {{site.scholar.bibliography}} %}

{% endif %}
</div>
