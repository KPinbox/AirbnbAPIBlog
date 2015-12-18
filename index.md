---
layout: page
title: Airbnb API Docs
tagline: The official unofficial docs
---

{% include JB/setup %}

{% for category in site.categories %}
	
	{% if category[0] == 'endpoint' %}

		{% assign endpoints = category[1] | sort: 'order' %}  
		{% include themes/nima/endpoints_toc %}
		{% include themes/nima/endpoints %}

	{% endif %}

{% endfor %}
