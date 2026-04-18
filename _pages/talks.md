---
layout: archive
title: "Talks and Posters"
permalink: /talks/
author_profile: true
---

## International Conference

### Oral

{% for post in site.talks reversed %}
  {% if post.category == "International" and post.type == "Oral" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}

### Poster

{% for post in site.talks reversed %}
  {% if post.category == "International" and post.type == "Poster" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}

---

## Domestic Conference

### Oral

{% for post in site.talks reversed %}
  {% if post.category == "Domestic" and post.type == "Oral" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}

### Poster

{% for post in site.talks reversed %}
  {% if post.category == "Domestic" and post.type == "Poster" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}