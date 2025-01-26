---
layout: default
title: Saggi in Italiano
---

# Saggi in Italiano

{% for post in site.pages %}
  {% if post.path contains 'italiano/' and post.layout == 'post' %}
  - [{{ post.title }}]({{ post.url }})
    <small>({{ post.date | date_to_string }})</small>
  {% endif %}
{% endfor %}