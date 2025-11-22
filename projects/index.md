---
layout: default
title: Projects
permalink: /projects/
---

## Projects

Below are the projects in the `projects` collection. Click a project to view its page.

<ul class="projects-list">
  {% for p in site.projects %}
    <li>
      <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
      {% if p.summary %}<p class="summary">{{ p.summary }}</p>{% endif %}
    </li>
  {% endfor %}
</ul>
