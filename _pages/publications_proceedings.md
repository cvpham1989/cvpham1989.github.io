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
  <a href="/publications_article">Journal</a>
  <a href="/publications_proceedings">Proceedings</a>
</div>
<div class="publications">
  {% bibliography -f {{site.scholar.bibliography}} --query @*[type=inproceedings] %} 
</div>
