---
layout: archive
title: "Mini Projects"
permalink: /mini-projects/
author_profile: true
---

{% include base_path %}

This page highlights applied analytical work across statistical learning, prediction,
financial modelling, and robust risk analysis. The emphasis is on how I approach
data problems, compare methods, and communicate results in a practical setting.

{% for post in site.mini_projects %}
  {% include archive-single.html %}
{% endfor %}
