---
layout: page
title: Magento Tutorial
description: 
permalink: /kb/magento/

---



<div class="container">
	<div class="row previews">
		{% for post in site.kb %}
		{% for category in post.categories %}
			{% if category == "magento" %}
				<div class="col-lg-12 col-sm-12">
					<a href="{{ site.url }}{{ post.url }}" class="post-image-link">
	                    <h2>{{ post.title }}</h2>
	                </a>

	                <p>{{ post.excerpt | strip_html }}</p>
				</div>	 
			{% endif %}
		{% endfor %}
		 
		{% endfor %}
	</div>
</div>