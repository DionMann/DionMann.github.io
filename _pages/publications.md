---
layout: archive
title: "Written Work"
permalink: /written-work/
author_profile: true
---

Here you can find a compilation of all my written work, including expository notes.

[Academic](#academic)  
[Notes](#notes)

# Academic
---
{% for post in site.publications reversed %}
  {% if post.pubtype == 'academic' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

# Notes
---
{% for post in site.publications reversed %}
  {% if post.pubtype == 'notes' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
