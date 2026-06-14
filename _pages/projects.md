---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: false
---

Research spanning multi-robot coordination, swarm intelligence, and autonomous systems—from learning-based controllers to physical robot platforms.

{% assign sorted_projects = site.projects | sort: "order" %}

<div class="projects-grid">
{% for project in sorted_projects %}
  {% include project-card.html project=project %}
{% endfor %}
</div>
