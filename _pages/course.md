---
layout: archive
title: "Courses"
permalink: /courses/
author_profile: true
---

{% include base_path %}

{% assign courses = site.courses | sort: 'date' | reverse %}

{% for course in courses %}
  {% include archive-single.html %}
{% endfor %}
