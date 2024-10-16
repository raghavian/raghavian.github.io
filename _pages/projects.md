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

## Key Project Areas

RS has been working in three key areas of Machine Learning research, with both methodological and application driven contributions.

- [Sustainability of AI](#sustainability-of-ai)
- [AI for Sciences](#ai-for-sciences)
- [Bio-Medical Image Analysis](#bio-medical-image-analysis)

## Sustainability of AI
---
Material cost of developing and deploying complex ML models is growing considerably. In this line of research, we are focusing on some facets of the environmental sustainability of ML. Primarily, by focusing on energy consumption and carbon footprint.

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
ML methods can accelerate research and open possibilities of asking novel questions in many scientific disciplines. In this line of research, several inter-disciplinary collaborations spanning a broad range of topics are being investigated. From an ML point of view, these do open interesting methods development.

<ol>
{% for post in site.publications reversed %}
  {% if post.project == 'ai4sciences' %}
     <li> {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>
---

## Bio-Medical Image Analysis
---
PhD training of RS was in medical image analysis. RS still holds keen interest in this domain and is active in investigating uncertainty quantification and use of deep latent generative models/ GNNs in this domain.

<ol>
{% for post in site.publications reversed %}
  {% if post.project == 'media' %}
     <li> {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>
---




