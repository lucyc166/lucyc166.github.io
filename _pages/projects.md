---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
---
<div style="text-align:center">
<font size ="+2"><b>Community Projects</b></font>
  <div class="row">
    {% assign sorted_projects = site.projects | sort: "importance" %}
    {% for project in sorted_projects %}
      <div class="col-xl-4 mt-3">
        {% if project.redirect %}
        <a href="{{ project.redirect }}" target="_blank">
        {% else %}
        <a href="{{ project.url | relative_url }}">
        {% endif %}

        <div class="view overlay">
          {% if project.img %}
          <img src="{{ project.img | relative_url }}" class = "img-fluid" alt="project thumbnail">
          {% endif %}
          <div class="mask flex-center rgba-red-strong">
            <p class="white-text">{{project.title}}</p>
          </div>
        </div>
        </a>
    </div>
  {% endfor %}
  </div>
</div>

<div style="text-align:center">
<font size ="+2"><b>Codefy Projects</b></font>
  <div class="row">
    {% assign sorted_projects = site.codefy | sort: "importance" %}
    {% for project in sorted_projects %}
      <div class="col-xl-4 mt-3">
        {% if project.redirect %}
        <a href="{{ project.redirect }}" target="_blank">
        {% else %}
        <a href="{{ project.url | relative_url }}">
        {% endif %}

        <div class="view overlay">
          {% if project.img %}
          <img src="{{ project.img | relative_url }}" class = "img-fluid" alt="project thumbnail">
          {% endif %}
          <div class="mask flex-center rgba-red-strong">
            <p class="white-text">{{project.title}}</p>
          </div>
        </div>
        </a>
    </div>
  {% endfor %}
  </div>
</div>

<div style="text-align:center">
<font size ="+2"><b>Coding Projects</b></font>
  <div class="row">
    {% assign sorted_projects = site.projects_code | sort: "importance" %}
    {% for project in sorted_projects %}
      <div class="col-xl-4 mt-3">
        {% if project.redirect %}
        <a href="{{ project.redirect }}" target="_blank">
        {% else %}
        <a href="{{ project.url | relative_url }}">
        {% endif %}

        <div class="view overlay">
          {% if project.img %}
          <img src="{{ project.img | relative_url }}" class = "img-fluid" alt="project thumbnail">
          {% endif %}
          <div class="mask flex-center rgba-red-strong">
            <p class="white-text">{{project.title}}</p>
          </div>
        </div>
        </a>
    </div>
  {% endfor %}
  </div>
</div>


<b>Coding Projects</b>
<div class="code projects grid fluid">
  {% assign sorted_projects = site.projects_code | sort: "importance" %}
  {% for project in sorted_projects %}
  <div class="grid-item">
    {% if project.redirect %}
    <a href="{{ project.redirect }}" target="_blank">
    {% else %}
    <a href="{{ project.url | relative_url }}">
    {% endif %}
      <div class="view overlay">
        {% if project.img %}
        <img src="{{ project.img | relative_url }}" class = "img-fluid" alt="project thumbnail">
        {% endif %}
        <div class="mask flex-center rgba-red-strong">
          <p class="white-text">{{project.title}}</p>
          <div class="row ml-1 mr-1 p-0">
            {% if project.github %}
            <div class="github-icon">
              <div class="icon" data-toggle="tooltip" title="Code Repository">
                <a href="{{ project.github }}" target="_blank"><i class="fab fa-github gh-icon"></i></a>
              </div>
              {% if project.github_stars %}
              <span class="stars" data-toggle="tooltip" title="GitHub Stars">
                <i class="fas fa-star"></i>
                <span id="{{ project.github_stars }}-stars"></span>
              </span>
              {% endif %}
            </div>
            {% endif %}
          </div>
        </div>
      </div>
    </a>
  </div>
{% endfor %}

</div>
