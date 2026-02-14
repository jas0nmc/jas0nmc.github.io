---
title: "8th Grade English"
permalink: /8th/english/
---

## Assignments

{% for post in site.posts %}
  {% if post.title %}
- [{{ post.title }}]({{ post.url }})
  {% endif %}
{% endfor %}
