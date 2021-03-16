---
layout: page
permalink: /publications/
title: publications
description:
years:
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
    <font size="-2"><a href="{{pub.url}}"><i class="fas fa-link"></i> Website </a></font>
    <font size="-2"><a href="/assets/pdf/{{pub.slug}}"><i class="far fa-file-pdf"></i> PDF</a>&nbsp;&nbsp;</font>


  </div>
  <br>
</div>

{% endfor %}

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded" src="{{ '/assets/img/cactus.png' | relative_url }}" alt=""/>
    </div>
</div>
