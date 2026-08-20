---
layout: default
title: "Projects"
permalink: /projects/
author_profile: true
---

<span class='anchor' id='projects'></span>

<div class="projects-page">

<div class="projects-page-intro" markdown="1">

This page highlights selected public GitHub projects, ordered by technical depth and relevance to AI engineering, machine learning, computer vision, NLP, scientific computing, GPU programming, and research software. Systems, web, networking, and software-engineering projects follow after the AI-focused work.

</div>

<div class="project-section-title">AI, Machine Learning, Computer Vision, NLP, Scientific Computing, and GPU Programming</div>

{% assign ai_projects = site.data.projects | where: "group", "ai" %}
{% for project in ai_projects %}
<div class='paper-box project-entry'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">{{ project.label }}</div>
      <img src='{{ project.image }}' alt="{{ project.title }} preview" width="400" height="225" loading="lazy">
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

<div class="project-section-title">Systems, Web, Networking, and Software Engineering</div>

{% assign systems_projects = site.data.projects | where: "group", "systems" %}
{% for project in systems_projects %}
<div class='paper-box project-entry'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">{{ project.label }}</div>
      <img src='{{ project.image }}' alt="{{ project.title }} preview" width="400" height="225" loading="lazy">
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
