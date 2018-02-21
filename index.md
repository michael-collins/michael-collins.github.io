---
layout: single
author_profile: false
classes:
  - front
header:
  overlay_color: "#000"
  overlay_filter: "0.25"
  overlay_image: /assets/images/header-bg.jpg
 
---
# Current Projects


[DMD Program](http://dmd.psu.edu)


[OER Schema](http://oerschema.org)

# Updates

{% for post in site.posts %}
<div class="row">
	<div class="small-12 columns">
  	
		<sub>{{ post.date | date: '%B %d, %Y' }}</sub>
		<a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>

	  	{{ post.excerpt }}

		<ul class="inline-list" style="margin-top:-1em;">
			{% for category in post.categories %}
			<li><h6><a href="/#!/{{ category }}"><i class="fa fa-tag"></i> {{ category }}</a></h6></li>
			{% endfor %}
		</ul>

	</div>
</div>
{% endfor %}