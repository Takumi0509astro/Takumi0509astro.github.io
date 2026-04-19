---
layout: archive
title: "発表文献"
permalink: /ja/publications/
author_profile: true
lang: ja
---

{% include base_path %}

{% if site.author.googlescholar %}
  <div class="wordwrap">Google Scholarのプロファイルでも論文リストを確認できます： <a href="{{site.author.googlescholar}}">Google Scholar</a></div>
{% endif %}

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% comment %} 日本語の記事のみを表示 {% endcomment %}
      {% if post.lang != "ja" %}{% continue %}{% endif %}
      {% if post.category != category[0] %}{% continue %}{% endif %}

      {% unless title_shown %}
        <h2>{{ category[1].title_ja | default: category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% if post.lang == "ja" %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}
{% endif %}