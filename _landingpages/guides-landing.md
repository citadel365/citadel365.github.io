---
layout: archive
permalink: /guides/
title: "Guides"
---

<div class="tiles">
	{% assign sorted_pages = site.pages | sort:"date" | reverse %}
	{% for page in sorted_pages %}
		{% if page.categories == "guides" %}
			{% include page-grid.html %}
		{% endif %} 
	{% endfor %}
</div>