---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

Preprints
---
<ol>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'preprint' %}
      <li> {% include archive-single.html %} <>
      </li>
  {% endif %}
{% endfor %}
</ol>


Journal Articles
---
{% for post in site.publications reversed %}
  {% if post.pubtype == 'journal' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

Refereed Conference/Workshop Papers
---
{% for post in site.publications reversed %}
  {% if post.pubtype == 'conference' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

Theses
---
{% for post in site.publications reversed %}
  {% if post.pubtype == 'thesis' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

