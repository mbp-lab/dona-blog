---
layout: page
permalink: /publications&repos/
title: publications & repositories
description: toDo description here
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->
<div class="publications">

{% bibliography %}

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}

</div>
