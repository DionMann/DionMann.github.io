---
layout: archive
title: "Written Work"
permalink: /written-work/
author_profile: true
---

[Academic](#academic)\
[Other](#other)

## Academic
{% for post in site.publications reversed %}
  {% if post.pubtype == 'academic' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Other
{% for post in site.publications reversed %}
  {% if post.pubtype == 'other' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
