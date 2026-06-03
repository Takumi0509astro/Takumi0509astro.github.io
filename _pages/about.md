---
layout: archive
permalink: /
lang: en
title: "Takumi Matsunaga / 松永拓巳"
author_profile: true
redirect_from:
  - /about/
  - /about.html
classes: home-title-center
---
<p align="center">
  <img src="/images/jaxa.jpg" width="60%">
</p>

I am a first-year Ph.D. student in the [Theoretical Astrophysics Group at Hokkaido University](https://astro3.sci.hokudai.ac.jp/huat/index.php/home_jp/).  
My research focuses on the formation and evolution of binary stars through numerical simulations, with particular interest in the origin of close Population III binaries that may become gravitational-wave sources.

## Research Overview

Population III stars, the first generation of stars in the Universe, are expected to form binary and multiple stellar systems. However, the processes that transform these primordial systems into close binaries, potential progenitors of gravitational-wave sources, remain poorly understood.

My research investigates how three-body interactions, angular momentum transport, and radiative feedback shape the orbital evolution of primordial stellar systems through numerical simulations.

## Current Research Topics

- Formation of close Population III binaries
- Three-body interactions in gaseous disks
- Angular momentum transport in primordial stellar systems
- Gravitational-wave progenitors from the first stars

## News

<ul class="news-list">
{% for n in site.data.news %}
  <li class="news-item">

    <span class="news-date">
      {{ n.date | date: "%b. %Y" }}
    </span>

    —

    {% if n.url %}
      <a href="{{ n.url }}" target="_blank" rel="noopener" class="news-link">
        {{ n.text }}
      </a>
    {% else %}
      <span class="news-text">
        {{ n.text }}
      </span>
    {% endif %}

  </li>
{% endfor %}
</ul>

## Upcoming Events

<ul>
{% for e in site.data.events %}
  <li>
    <strong>
      {{ e.date | date: "%b. %-d" }}
      {% if e.date_end %}
        –{{ e.date_end | date: "%-d, %Y" }}
      {% else %}
        , {{ e.date | date: "%Y" }}
      {% endif %}
    </strong>
    —
    <a href="{{ e.url }}" target="_blank" rel="noopener">
      {{ e.title }}
    </a>
    ({{ e.location }})
  </li>
{% endfor %}
</ul>

## Contact

matsunaga[at]astro1.sci.hokudai.ac.jp  
(Please replace "[at]" with "@".)