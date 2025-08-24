---
layout: archive
title: "Written Work"
permalink: /written-work/
author_profile: true
---

Here you can find a compilation of all my written work, including expository notes. Click on the title of the paper you are interested in to get a more detailed explanation, or you can just click the _Download Paper_ button for the full pdf!

[Notes](#notes)  
[Other Academic Work](#other-academic-work)

---

# Notes

---

{% for post in site.publications reversed %}
  {% if post.pubtype == 'notes' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

---

# Other Academic Work  
Here you can find miscellaneous work, such as problems/exercises from various areas of math.

---

{% for post in site.publications reversed %}
  {% if post.pubtype == 'other' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

---
