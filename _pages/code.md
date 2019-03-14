---
layout: archive
title: "Code"
permalink: /code/
author_profile: true
---

{% include base_path %}

{% for post in site.code reversed %}  
  {% if post.collection == 'code' %}  
    {% include archive-single.html %}  
  {% endif %}  
{% endfor %}  
