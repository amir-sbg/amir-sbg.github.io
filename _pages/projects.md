---
layout: default
title: "Projects"
permalink: /projects/
author_profile: true
---

<span class='anchor' id='projects'></span>

<div class="projects-page">

<div class="projects-page-intro" markdown="1">

This page organizes my GitHub projects by technical depth and research relevance. Machine learning, computer vision, NLP, data science, and AI-oriented projects are listed first, followed by systems, web, networking, and programming projects.

</div>

<div class="project-section-title">Machine Learning, Computer Vision, and Data Science</div>

{% assign ai_projects = site.data.projects | where: "group", "ai" %}
{% for project in ai_projects %}
<div class='paper-box project-entry'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">{{ project.label }}</div>
      <img src='{{ project.image }}' alt="{{ project.title }} preview" width="100%" loading="lazy">
      {% if project.venue_image %}
      <img class="venue-mark" src='{{ project.venue_image }}' alt="{{ project.venue_alt | default: project.label }}" loading="lazy">
      {% endif %}
    </div>
  </div>
  <div class='paper-box-text'>
    <h2 class="project-entry-title"><a href="{{ project.repo }}">{{ project.title }}</a></h2>
    <div class="project-entry-meta">{{ project.year }} &nbsp;|&nbsp; {{ project.stack }}</div>
    <p>{{ project.description }}</p>
  </div>
</div>
{% endfor %}

<div class="project-section-title">Systems, Web, Networking, and Programming</div>

{% assign systems_projects = site.data.projects | where: "group", "systems" %}
{% for project in systems_projects %}
<div class='paper-box project-entry'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">{{ project.label }}</div>
      <img src='{{ project.image }}' alt="{{ project.title }} preview" width="100%" loading="lazy">
      {% if project.venue_image %}
      <img class="venue-mark" src='{{ project.venue_image }}' alt="{{ project.venue_alt | default: project.label }}" loading="lazy">
      {% endif %}
    </div>
  </div>
  <div class='paper-box-text'>
    <h2 class="project-entry-title"><a href="{{ project.repo }}">{{ project.title }}</a></h2>
    <div class="project-entry-meta">{{ project.year }} &nbsp;|&nbsp; {{ project.stack }}</div>
    <p>{{ project.description }}</p>
  </div>
</div>
{% endfor %}

</div>
