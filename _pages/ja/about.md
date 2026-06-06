---
layout: archive
permalink: /ja/
lang: ja
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

北海道大学大学院理学院宇宙理学専攻の博士後期課程1年です。  
所属は[理論天文学研究室](https://astro3.sci.hokudai.ac.jp/huat/index.php/home_jp/)です。

数値シミュレーションを用いて連星形成とその進化過程を研究しています。特に、重力波源となる可能性のある初代星近接連星の起源に関心を持っています。

## 研究概要

宇宙で最初に誕生した恒星である初代星（Population III stars）は、連星や多重星系を形成すると考えられています。しかし、これらの始原的な星系がどのような過程を経て重力波源の前駆天体となる近接連星へと進化するのかは、十分に解明されていません。

私は数値シミュレーションを用いて、三体相互作用、角運動量輸送、放射フィードバックが初代星系の軌道進化に与える影響を調べています。

## 現在の研究テーマ

- 初代星近接連星の形成
- ガス円盤中における三体相互作用
- 初代星系における角運動量輸送
- 初代星起源の重力波源形成

## お知らせ

<ul class="news-list">
{% for n in site.data.news %}
  <li class="news-item">

    <span class="news-date">
      {{ n.date | date: "%Y年%-m月" }}
    </span>

    —

    {% if n.url %}
      <a href="{{ n.url }}" target="_blank" rel="noopener" class="news-link">
        {{ n.textja }}
      </a>
    {% else %}
      <span class="news-text">
        {{ n.textja }}
      </span>
    {% endif %}

  </li>
{% endfor %}
</ul>

## 今後の予定

<ul>
{% for e in site.data.events %}
  <li>
    {{ e.date | date: "%Y/%m/%d" }}
    {% if e.date_end %}
      –{{ e.date_end | date: "%d" }}
    {% endif %}
    —
    <a href="{{ e.url }}" target="_blank" rel="noopener">
      {{ e.title }}
    </a>
    （{{ e.location }}）
  </li>
{% endfor %}
</ul>

## 連絡先

matsunaga[at]astro1.sci.hokudai.ac.jp  
※ [at] を @ に置き換えてください。