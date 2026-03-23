---
layout: page
permalink: /repositories/
title: software
description: R packages and GitHub repositories
nav: true
nav_order: 5
---

{% if site.data.repositories.github_repos %}

## R Packages

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
