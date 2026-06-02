---
layout: archive
title: "Presentations"
permalink: /talks/
lang: en
author_profile: true
---

## International Conference

### Oral
<ul>
{% for post in site.talks reversed %}
  {% if post.category == "International" and post.type == "Oral" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}
</ul>

### Poster
<ul>
{% for post in site.talks reversed %}
  {% if post.category == "International" and post.type == "Poster" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}
</ul>
---

## Domestic Conference

### Oral
<ul>
{% for post in site.talks reversed %}
  {% if post.category == "Domestic" and post.type == "Oral" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}
</ul>

### Poster
<ul>
{% for post in site.talks reversed %}
  {% if post.category == "Domestic" and post.type == "Poster" %}
    {% include archive-single-talk.html %}
  {% endif %}
{% endfor %}
</ul>