---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: [1956, 1950, 1935, 1905]
nav: true
---

<div class="publications">
<div style = 'margin-right;'>
{% assign publications = site.publications | sort: "year" | reverse %}
{% for pub in publications %}
<div class="pubitem">
  <div class="pubtitle">
    <b>{{ pub.title }}</b>
  </div>
  <div class="pubauthors">
    <font size="-2">{{ pub.authors }}</font>
  </div>
  <div class="pubinfo">
    <font size="-2">{{ pub.publication }}, {{ pub.year}}</font>
  </div>
  <div class="publinks">
    {% if pub.slug %}
      <font size="-2"><a href="/assets/pdf/{{pub.slug}}"><i class="far fa-file-pdf"></i> PDF</a>&nbsp;&nbsp;</font>
    {% endif %}
    {% if pub.url %}
    <font size="-2"><a href="{{pub.url}}"><i class="fas fa-link"></i> Project Page</a></font>
    {% else %}
    <font size="-2"> </font>
    {% endif %}
  </div>
</div>
</div>

{% endfor %}
