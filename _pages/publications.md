---
layout: archive
title: "Written Work"
permalink: /written-work/
author_profile: true
---

Here you can find a compilation of all my written work, including expository notes.

[Notes](#notes)  
[Other Academic Work](#other-academic-work)

# Notes

---

{% for post in site.publications reversed %}
  {% if post.pubtype == 'notes' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

---

# Other Academic Work  
Here you can find miscellaneous work, such as excercises from various areas of math.  

---

{% for post in site.publications reversed %}
  {% if post.pubtype == 'other' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

---
