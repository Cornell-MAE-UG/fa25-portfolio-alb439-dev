---
layout: default
title: <Ari Ben-Zvi> - Portfolio
permalink: /projects/
---

<div class="gallery-container">
<div class="project-gallery">
    {% assign projects_sorted = site.projects | sort: "order" %}
    {% for project in projects_sorted %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          <p>{{ project.title }}</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>