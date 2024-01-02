---
layout: page
permalink: /publications_proceedings/
title: Publications
description: #
nav: false
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="filter-buttons">
  <a href="/publications" style="color:var(--global-text-color)">All</a>
  <a href="/publications_article" style="color:var(--global-text-color)">Journal</a>
  <a href="/publications_proceedings">Proceedings</a>
</div>
<div class="publications">
{% bibliography -f {{site.scholar.bibliography}} --query @*[type=inproceedings] %} 
</div>
