---
layout: archive
title: "Code"
permalink: /code/
author_profile: true
redirect_from:
  - /code
---

{% include base_path %}

In Progress
===========

This is a WIP
{% for post in site.publications reversed %}
  {% if post.collection == 'publications' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
