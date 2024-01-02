---
layout: page
permalink: /publications_article/
title: Publications
description: #
nav: false
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="filter-buttons">
  <a href="/publications" style="color:var(--global-text-color)">All</a>
  <a href="/publications_article">Journal</a>
  <a href="/publications_proceedings" style="color:var(--global-text-color)">Proceedings</a>
</div>
<div class="publications">
{% bibliography -f {{site.scholar.bibliography}} --query @*[type=article] %}
</div>
