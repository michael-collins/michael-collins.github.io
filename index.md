---
layout: single
author_profile: false
classes:
  - front
header:
  overlay_color: "#37c6fd"
  overlay_filter: "0.10"
  overlay_image: /assets/images/front-banner.jpg
 
---
# Recent

## OER Camp, 2018

[Workshop Recap by Katrina Wehr](https://medium.com/@katrina.m.wehr/oer-camp-2018-summary-2c8b34a3f341)

[Workshop documentation](https://open-curriculum.gitbooks.io/oer-camp-2018/content/)

**Related project:**

[OER Schema]({{ "portfolio/oerschema/" | prepend: site.baseurl }})

<!-- # Updates -->

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