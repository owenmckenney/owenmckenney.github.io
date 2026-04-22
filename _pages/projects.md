---
layout: page
title: other projects
permalink: /projects/
description: Selected projects and reports. [See other assorted technical work here](/assets/pdf/Owen-McKenney-Technical-Portfolio.pdf)
nav: true
nav_order: 3
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  {% assign standard_projects = sorted_projects | where_exp: "project", "project.is_report != true" %}
  {% assign report_projects = sorted_projects | where_exp: "project", "project.is_report == true" %}

  {% if page.horizontal %}
    {% if standard_projects.size > 0 %}
      <div class="container">
        <div class="row row-cols-1 row-cols-md-2">
          {% for project in standard_projects %}
            {% include projects_horizontal.liquid %}
          {% endfor %}
        </div>
      </div>
    {% endif %}

    {% if report_projects.size > 0 %}
      <h1 class="post-title projects-section-title">reports</h1>
      <div class="container">
        <div class="row row-cols-1 row-cols-md-2">
          {% for project in report_projects %}
            {% include projects_horizontal.liquid %}
          {% endfor %}
        </div>
      </div>
    {% endif %}
  {% else %}
    {% if standard_projects.size > 0 %}
      <div class="row row-cols-1 row-cols-md-3">
        {% for project in standard_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
    {% endif %}

    {% if report_projects.size > 0 %}
      <h1 class="post-title projects-section-title">reports</h1>
      <div class="row row-cols-1 row-cols-md-3">
        {% for project in report_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
    {% endif %}
  {% endif %}
</div>
