---
layout: page
title: projects
permalink: /projects/
description: UX/UI and data projects in HCI, accessibility, and analytics.
nav: true
nav_order: 3
display_categories: []
horizontal: false
_styles: >
  .projects .row { row-gap: 0; }
  .project-row-link { text-decoration: none !important; color: inherit; display: block; }
  .project-row {
    position: relative;
    display: flex;
    align-items: center;
    gap: 20px;
    background: var(--global-card-bg-color, #fff);
    border: 1px solid var(--global-divider-color, #e6e6e6);
    border-radius: 10px;
    padding: 22px 26px;
    transition: transform 0.15s ease, box-shadow 0.15s ease, border-color 0.15s ease;
    overflow: hidden;
  }
  .project-row:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
    border-color: var(--global-theme-color);
  }
  .project-row-body { flex: 1; min-width: 0; }
  .project-row-header {
    display: flex;
    flex-wrap: wrap;
    align-items: baseline;
    justify-content: space-between;
    gap: 8px;
  }
  .project-row-title { font-size: 1.15rem; margin: 0; font-weight: 700; }
  .project-row-period {
    font-size: 0.78rem;
    color: var(--global-text-color-light, #6b6b6b);
    white-space: nowrap;
    font-style: italic;
  }
  .project-row-org {
    font-size: 0.82rem;
    color: var(--global-text-color);
    font-weight: 600;
    margin-top: 2px;
  }
  .project-row-text {
    margin: 8px 0 0;
    font-size: 0.92rem;
    color: var(--global-text-color, #444);
  }
  .project-row-arrow {
    flex-shrink: 0;
    color: var(--global-text-color-light, #999);
    font-size: 1.1rem;
    opacity: 0;
    transform: translateX(-6px);
    transition: opacity 0.15s ease, transform 0.15s ease;
  }
  .project-row:hover .project-row-arrow {
    opacity: 1;
    transform: translateX(0);
    color: var(--global-theme-color);
  }
  @media (max-width: 576px) {
    .project-row { flex-direction: column; align-items: stretch; padding: 18px 20px; }
    .project-row-arrow { display: none; }
  }
---

<div class="projects">
{% assign sorted_projects = site.projects | sort: "importance" %}
<div class="row row-cols-1">
{% for project in sorted_projects %}
  {% include projects.liquid %}
{% endfor %}
</div>
</div>
