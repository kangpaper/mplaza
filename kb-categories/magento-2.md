---
layout: page
title: Magento 2
description: 
permalink: /kb/magento-2/

---



<div class="container">
	<div class="row previews">
		{% for post in site.kb %}
		{% for category in post.categories %}
			{% if category == "magento-2" %}
				<div class="col-lg-4 col-sm-6">
					<div class="thumbnail">
						
						<div class="caption">
							<a href="{{ site.url }}{{ post.url }}" class="post-image-link">
			                    <h3>{{ post.title }}</h3>
			                </a>
						</div>
					</div>
				</div>	 
			{% endif %}
		{% endfor %}
		 
		{% endfor %}
	</div>
</div>