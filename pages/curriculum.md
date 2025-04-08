---
layout: archive
title: Curriculum
permalink: /curriculum/
author_profile: false
classes:
  - curriculum-theme
breadcrumbs: false
---

<h3>Programs</h3>
<div class="grid__wrapper"> 
{% assign items = site.curriculum | where:"category","programs" | sort: 'year' | reverse  %}
{% for post in items %}
{% include archive-single.html type="grid" %}
{% endfor %}
</div> 

<h3>Courses</h3>
<div class="grid__wrapper">
{% assign items = site.curriculum | where:"category","courses" | sort: 'year' | reverse %}
{% for post in items %}

{% include archive-single.html type="grid" %}
{% endfor %}
</div>


