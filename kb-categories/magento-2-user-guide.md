---
layout: kb
title: Magento 2 User Guide
description: 
permalink: /kb/magento-2-user-guide/

---



<div class="container">
	<div class="row previews">
		{% for post in site.kb.m2-userguide %}
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