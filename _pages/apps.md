---
layout: page
title: apps
permalink: /apps/
description: A growing collection of apps I've built.
nav: true
nav_order: 9
horizontal: false
---

<!-- pages/apps.md -->
<div class="projects">
{% assign sorted_apps = site.projects | where: "category", "apps" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3">
{% for project in sorted_apps %}
  {% include projects.liquid %}
{% endfor %}
</div>
</div>
