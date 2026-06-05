---
layout: archive
title: "Teaching"
permalink: /teaching/
lang: en
author_profile: true
---

## Teaching Assistant
<ul>
{% for post in site.teaching reversed %}
  {% if post.type == "Teaching Assistant" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
</ul>