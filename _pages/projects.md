---
layout: page
title: projects
permalink: /projects/
description: Selected GenAI, data, and automation projects.
nav: true
nav_order: 3
display_categories: [work, fun]
---

<style>
  .project-index {
    display: grid;
    gap: 2.25rem;
  }

  .project-index__category {
    margin-bottom: 1rem;
    color: var(--global-theme-color);
    font-size: 0.9rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  .project-index__list {
    display: grid;
    gap: 0;
    border-top: 1px solid var(--global-divider-color);
  }

  .project-index__item {
    display: grid;
    grid-template-columns: minmax(11rem, 0.8fr) 1.4fr;
    gap: 1.5rem;
    min-height: 7.5rem;
    padding: 1.35rem 0;
    border-bottom: 1px solid var(--global-divider-color);
  }

  .project-index__title {
    margin: 0;
    font-family: "Roboto Slab", Georgia, serif;
    font-size: 1.15rem;
    font-weight: 400;
    line-height: 1.35;
    text-transform: none;
  }

  .project-index__link {
    color: var(--global-text-color);
  }

  .project-index__description {
    margin: 0;
    color: var(--global-text-color-light);
    line-height: 1.65;
  }

  .project-index__meta {
    display: block;
    margin-top: 0.45rem;
    color: var(--global-theme-color);
    font-family: "Roboto Slab", Georgia, serif;
    font-size: 0.84rem;
    font-style: italic;
    font-weight: 300;
    letter-spacing: 0.01em;
    line-height: 1.5;
  }

  .project-index__meta-label {
    color: var(--global-text-color-light);
    font-style: italic;
    font-weight: 300;
  }

  .project-index__link:hover {
    text-decoration: none;
  }

  @media (max-width: 768px) {
    .project-index__item {
      grid-template-columns: 1fr;
      gap: 0.65rem;
      min-height: 0;
    }
  }
</style>

<div class="project-index">
{%- if site.enable_project_categories and page.display_categories %}
  {%- for category in page.display_categories %}
    {%- assign categorized_projects = site.projects | where: "category", category -%}
    {%- assign sorted_projects = categorized_projects | sort: "importance" %}
    <section>
      <h2 class="project-index__category">{{ category }}</h2>
      <div class="project-index__list">
        {%- for project in sorted_projects %}
          <article class="project-index__item">
            <h3 class="project-index__title">
              {%- if project.redirect %}
                <a class="project-index__link" href="{{ project.redirect }}">{{ project.title }}</a>
              {%- else %}
                <a class="project-index__link" href="{{ project.url | relative_url }}">{{ project.title }}</a>
              {%- endif %}
            </h3>
            <div>
              <p class="project-index__description">{{ project.description }}</p>
              {%- if project.tech_stack %}
                <span class="project-index__meta">
                  <span class="project-index__meta-label">tech:</span>
                  {{ project.tech_stack | join: " / " }}
                </span>
              {%- endif %}
            </div>
          </article>
        {%- endfor %}
      </div>
    </section>
  {%- endfor %}
{%- else %}
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <section>
    <div class="project-index__list">
      {%- for project in sorted_projects %}
        <article class="project-index__item">
          <h3 class="project-index__title">
            {%- if project.redirect %}
              <a class="project-index__link" href="{{ project.redirect }}">{{ project.title }}</a>
            {%- else %}
              <a class="project-index__link" href="{{ project.url | relative_url }}">{{ project.title }}</a>
            {%- endif %}
          </h3>
          <div>
            <p class="project-index__description">{{ project.description }}</p>
            {%- if project.tech_stack %}
              <span class="project-index__meta">
                <span class="project-index__meta-label">tech:</span>
                {{ project.tech_stack | join: " / " }}
              </span>
            {%- endif %}
          </div>
        </article>
      {%- endfor %}
    </div>
  </section>
{%- endif %}
</div>
