---
layout: archive
title: "Talks and Presentations"
permalink: /talks/
author_profile: true
---

## International Conference

### Oral Presentations

{% for post in site.talks reversed %}
  {% if post.category == "International" and post.type == "Oral" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}

### Poster Presentations

{% for post in site.talks reversed %}
  {% if post.category == "International" and post.type == "Poster" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}

---

## Domestic Conference

### Oral Presentations

{% for post in site.talks reversed %}
  {% if post.category == "Domestic" and post.type == "Oral" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}

### Poster Presentations

{% for post in site.talks reversed %}
  {% if post.category == "Domestic" and post.type == "Poster" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}