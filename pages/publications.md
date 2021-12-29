---
layout: archive
title: Publications
permalink: /publications/
author_profile: false
classes:
  - curriculum-theme
breadcrumbs: false
---

<h3>Book Chapters</h3>
<div class="grid__wrapper"> 
{% assign items = site.publications | where:"category","chapters" | sort: 'year' | reverse  %}
{% for post in items %}
{% include archive-single.html type="grid" %}
{% endfor %}
</div> 


