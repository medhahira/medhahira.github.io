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
  ### [{{ projects.title }}]({{ projects.github_link }})
  
  **Description:** {{ projects.description }}
  
  **Tech Stack:** {{ projects.tech_stack }}
  
  {% include archive-projects.html %}
{% endfor %}

