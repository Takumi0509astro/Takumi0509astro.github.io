---
layout: archive
title: "CV"
permalink: /cv/
lang: en
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education

**Doctor of Science (Cosmosciences)**  
Graduate School of Science, Hokkaido University, Japan  
April 2026 – Present  
(Expected completion: March 2029)

**Master of Science (Astrophysics)**  
Graduate School of Science and Engineering, Ibaraki University, Japan  
April 2024 – March 2026

**Bachelor of Science (Physics)**  
College of Science, Ibaraki University, Japan  
April 2020 – March 2024

**High school**  
Chiba Prefectural Funabashi High School (Science Course), Japan  
April 2017 – March 2020


## Fellowships and Awards
**Hokkaido University EXEX Doctoral Fellowship**  
April 2026 – March 2029


## Research Interests
- Binary star formation  
- Star formation  
- Angular momentum distribution in molecular clouds  
- Computational astrophysics  


## Skills
- **Programming**: Python, C  
- **Simulation**: Smoothed Particle Hydrodynamics (SPH), Gadget  
- **Tools**: Linux, Git, LaTeX  


## Publications
<ul>
{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>


## Talks and Presentations
<ul>
{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}
</ul>


## Teaching Experience
<ul>
{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>