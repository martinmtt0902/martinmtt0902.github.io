---
layout: archive
title: "Mini Projects"
permalink: /mini-projects/
author_profile: true
---

{% include base_path %}

Here is a selection of smaller projects and course assessments.

{% for post in site.mini_projects reversed %}
  {% include archive-single.html %}
{% endfor %}
