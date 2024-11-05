---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

{% for project in site.projects %}
  ### [{{ project.title }}]({{ project.github_link }})
  
  **Description:** {{ project.description }}
  
  **Tech Stack:** {{ project.tech_stack }}
  
  {% include archive-single.html %}
{% endfor %}
