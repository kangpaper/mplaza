---
layout: page
title: Magento 2 Tutorial
description: 
permalink: /kb/magento-2-tutorial/

---



<div class="container">
	<div class="row previews">
		{% for post in site.kb.categories.m2 %}
		<div class="col-lg-4 col-sm-6">
			<div class="thumbnail">
				
				<div class="caption">
					<a href="{{ site.url }}{{ post.url }}" class="post-image-link">
	                    <h3>{{ post.title }}</h3>
	                </a>
				</div>
			</div>
		</div>	  
		{% endfor %}
	</div>
</div>