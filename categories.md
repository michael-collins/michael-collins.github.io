---
layout: archive
permalink: /categories/
title:
author_profile: false
---

{% include group-by-array collection=site.portfolio field="categories" %}

{% for category in group_names %}
  {% assign categories = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
 
  {% for categories in site.portfolio %}
    
  {% endfor %}
{% endfor %}