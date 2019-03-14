---
layout: archive
title: "Code"
permalink: /code/
author_profile: true

---

{% include base_path %}

### In Progress...

*This is a WIP - Look at my GitHub repos in the meantime :)*
{% for post in site.code reversed %}  
  {% if post.collection == 'code' %}  
    {% include archive-single.html %}  
  {% endif %}  
{% endfor %}  
