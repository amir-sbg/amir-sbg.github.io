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
      {% if project.animated_image %}
      <a class="paper-box-media-swap" href="{{ project.project_url | default: project.repo }}"><img class="media-swap-static" src='{{ project.image }}' alt="{{ project.title }} preview" width="400" height="225"><img class="media-swap-animated" src='{{ project.animated_image }}' alt="" aria-hidden="true" width="400" height="225" loading="lazy" onload="this.parentElement.classList.add('is-loaded')"></a>
      {% else %}
      {% if project.project_url %}<a href="{{ project.project_url }}">{% endif %}<img src='{{ project.image }}' alt="{{ project.title }} preview" width="400" height="225" loading="lazy">{% if project.project_url %}</a>{% endif %}
      {% endif %}
      {% if project.venue_image %}
      <img class="venue-mark" src='{{ project.venue_image }}' alt="{{ project.venue_alt | default: project.label }}" loading="lazy">
      {% endif %}
    </div>
  </div>
  <div class='paper-box-text'>
    <h2 class="project-entry-title"><a href="{{ project.project_url | default: project.repo }}">{{ project.title }}</a></h2>
    <div class="project-entry-meta">{{ project.year }} &nbsp;|&nbsp; {{ project.stack }}</div>
    <p>{{ project.description }}</p>
    {% if project.publication %}
    <p class="project-publication-links">
      {{ project.venue_status }} <a href="{{ project.venue_url }}">{{ project.venue_name }}</a>{% if project.workshop_url %} (<a href="{{ project.workshop_url }}">{{ project.workshop_name }}</a>){% endif %}{% if project.acceptance %} &middot; Acceptance ratio: {{ project.acceptance }}{% endif %}<br>
      <em>{{ project.date }}</em> &middot; First author<br>
      Project: <a href="{{ project.project_url }}">Website</a> &middot; Code: <a href="{{ project.repo }}">GitHub</a>{% if project.arxiv_url %} &middot; arXiv: <a href="{{ project.arxiv_url }}">{{ project.arxiv_label }}</a>{% elsif project.arxiv_label %} &middot; arXiv: {{ project.arxiv_label }}{% endif %}{% if project.openreview_url %} &middot; <a href="{{ project.openreview_url }}">OpenReview</a>{% endif %}{% if project.doi_url %} &middot; DOI: <a href="{{ project.doi_url }}">{{ project.doi_label }}</a>{% endif %}
    </p>
    {% elsif project.project_url %}
    <p class="project-publication-links">Project: <a href="{{ project.project_url }}">Website</a> &middot; Code: <a href="{{ project.repo }}">GitHub</a></p>
    {% endif %}
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
