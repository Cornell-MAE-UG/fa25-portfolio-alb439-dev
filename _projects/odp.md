---
layout: default
title: "ODP"
description: ODP sub-projects
order: 3
technologies: []
permalink: /odp/
---

<div class="gallery-container">
<div class="project-gallery">
    {% assign odp_sorted = site.odp | sort: "order" %}
    {% for project in odp_sorted %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          <p>{{ project.title }}</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>

<a href="{{ '/projects/' | relative_url }}" class="back-arrow">
    <i class="bi bi-arrow-left-circle-fill"></i> Back to Projects
</a>