---
layout: projects
title: Projects
permalink: /projects/
---

  <div class="work">
    <h2>My Work</h2>
    {% for project in site.portfolio %}
    <div class="project">
      <div class="project-thumb">
        <a href="{{ project.url | prepend: site.baseurl }}">
          <img src="/img/{{ project.grid }}.png" alt="{{ project.title }}"/> 
        </a>
      </div>
      <div class="project-description">
        <a href="{{ project.url | prepend: site.baseurl }}"><strong>{{ project.title }}</strong></a>
        <p>{{ project.short-description }}</p>
      </div>
    </div>
    {% endfor %}
  </div>
  