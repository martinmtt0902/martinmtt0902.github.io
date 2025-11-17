---
layout: archive
title: "Mini Projects"
permalink: /mini-projects/
author_profile: true
---

{% include base_path %}

Here is a selection of smaller projects and course assessments.

{% for proj in site.mini_projects %}
  {% include archive-single.html %}
{% endfor %}
