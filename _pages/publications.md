---
layout: archive
title: "Written Work"
permalink: /written-work/
author_profile: true
---

Here you can find a compilation of all my written work, including expository notes.

[Academic](#academic)\
[Other](#other)

# Academic
---
{% for post in site.publications reversed %}
  {% if post.pubtype == 'academic' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

# Other
---
{% for post in site.publications reversed %}
  {% if post.pubtype == 'other' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
