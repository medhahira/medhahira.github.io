---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---
{% if author.github %}
  You can also find my projects on <u><a href="{{author.github}}">my Github profile</a>.</u>
{% endif %}

{% include base_path %}

{% for project in site.port %}
  ### [{{ project.title }}]({{ project.github_link }})
  
  **Description:** {{ project.description }}
  
  **Tech Stack:** {{ project.tech_stack }}
  
  {% include archive-single.html %}
{% endfor %}

