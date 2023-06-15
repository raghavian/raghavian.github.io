---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}
{% if author.googlescholar %}
You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

## Sustainability of AI
---
<ol>
{% for post in site.publications reversed %}
  {% if post.project == 'sustofai' %}
     <li> {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>

---

## AI for Sciences
---
<ol>
{% for post in site.publications reversed %}
  {% if post.project == 'ai4sciences' %}
     <li> {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>
---

## Medical Image Analysis
---
<ol>
{% for post in site.publications reversed %}
  {% if post.project == 'media' %}
     <li> {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>
---




