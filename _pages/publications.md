---
layout: page
title: "Publications"
permalink: /publications/
subtitle: "* denotes equal contribution."
---

<p><a href="{{ site.author.googlescholar }}">View my Google Scholar profile →</a></p>

<div class="pub-list">
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for post in pubs %}
  {% include publication-item.html %}
{% endfor %}
</div>
