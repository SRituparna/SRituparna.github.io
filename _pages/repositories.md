---
layout: page
permalink: /repositories/
title: repositories
description: Library of my open-sourced contribution
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
{% if site.data.repositories.github_users.size > 1 %}

  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.liquid username=user %}
  </div>

<!-- ---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_repos %} -->

<!-- ## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %} -->

---

## Observable

<iframe width="100%" height="800" frameborder="0"
  src="https://observablehq.com/embed/1c11066aa24ae815@150?cells=embed&api_key=63fce89c77f67a4bc12e29bc19e9dd7fba697ad8"></iframe>

---

## Notion Template

<iframe src="https://personalaccountsofameteorologist.notion.site/ebd//64c563ec53a544699d572c9f04bc8dab?v=c4410bb809164632b918eeb9da594358" width="100%" height="600" frameborder="0" allowfullscreen>
