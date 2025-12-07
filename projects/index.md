---
layout: default
title: Projects
permalink: /projects/
---
<style>
body {
    background-color: #f7f7f7; /* whole page background */
}

.site-header {
    background-color: #ffffff; /* navigation/header */
    border-bottom: 1px solid #e0e0e0;
}

.site-footer {
    background-color: #ffffff; /* footer */
    border-top: 1px solid #e0e0e0;
}

.page-content {
    background-color: #f7f7f7; /* main content area */
}
</style>

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
