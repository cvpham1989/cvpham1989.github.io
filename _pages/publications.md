---
layout: page
permalink: /publications/
title: Publications
description: #
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">
{% if page.params.type == 'inproceedings' or page.params.type == 'article' %}
  {% bibliography -f {{site.scholar.bibliography}} --query @*[type={{page.params.type}}] %}
{% else %}
  {% bibliography -f {{site.scholar.bibliography}} %}
{% endif %}
</div>
