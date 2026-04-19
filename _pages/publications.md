---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
lang: en
---

{% include base_path %}

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% comment %} 英語の記事のみを表示 {% endcomment %}
      {% if post.lang != "en" and post.lang != nil %}{% continue %}{% endif %}
      {% if post.category != category[0] %}{% continue %}{% endif %}

      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% if post.lang == "en" or post.lang == nil %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}
{% endif %}