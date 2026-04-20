---
layout: archive
title: "経歴"
permalink: /ja/cv/
lang: ja
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## 学歴

**博士（理学）**  
北海道大学 大学院理学院 宇宙理学専攻  
2026年4月 – 現在  
（修了予定：2029年3月）

**修士（理学）**  
茨城大学 大学院理工学研究科 理学専攻 宇宙物理学コース  
2024年4月 – 2026年3月

**学士（理学）**  
茨城大学 理学部 理学科 物理学コース  
2020年4月 – 2024年3月

**高等学校**  
千葉県立船橋高等学校（理数科）  
2017年4月 – 2020年3月


## フェローシップ・受賞

**北海道大学 EXEX博士人材フェローシップ**  
2026年4月 – 2029年3月


## 研究分野

- 連星形成  
- 星形成  
- 分子雲における角運動量分布  
- 計算宇宙物理学  


## スキル

- **プログラミング**：Python, C  
- **数値計算**：Smoothed Particle Hydrodynamics (SPH), GADGETコード  
- **ツール**：Linux, Git, LaTeX  


## 論文
<ul>
{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>


## 研究発表
<ul>
{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}
</ul>


## 教育経験
<ul>
{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>