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

## EDUI Conference, 2018

Slides: [REMIXING OPEN CONTENT + PEDAGOGY WITH OERSCHEMA](https://docs.google.com/presentation/d/e/2PACX-1vSul0t5D8mE7e_pQqHd-7XKMBwMiNWvlX_qkBzwnurM0zcbcrM0EkylM1T8EpzPKJwcxXfC5uAcsrPs/pub?start=false&loop=false&delayms=3000)

## MADE Symposium, 2018

Slides: [MADE Symposium Design Thinking Workshop](https://docs.google.com/presentation/d/e/2PACX-1vTcsV4orqbKRF14ArwJybb-8LIC4eFkp0rVE07Qm_hhpcrVIfnXAKbnarO_KCSrXGBAa9S9ABvHSHri/pub?start=false&loop=false&delayms=3000)

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