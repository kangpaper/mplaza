---
layout: page
title: Magento 2 Tutorial
description: 
permalink: /kb/magento-2-tutorial/

---



<div class="container">

	<div class="row">
	<p>
		Magento 2 was released with improved performance and better code base than the previous version. In addition, Magento 2 supports new features to boost conversion rates more effectively, and business agility and productivity improvements. These Magento 2 tutorials cover back and front-end development, as well as administration guides to help you get up and running with Magento 2. For the whole eCommerce community, this is a real boom! Magento 1.x has been around for nearly 10 years and it’s very obvious that it needed either a major update or complete replacement.


		</p>

		<p>Are you Magento developers or merchant, you are going to learn more about Magento 2, yes it is place for you.
		</p>
	</div>
	
	<div class="row previews">
		{% for post in site.kb %}
		{% for category in post.categories %}
			{% if category == "magento-2-tutorial" %}
				<div class="col-lg-12 col-sm-12">
					<a href="{{ site.url }}{{ post.url }}" class="post-image-link">
	                    <h2>{{ post.title }}</h2>
	                </a>

	                <p>{{ post.excerpt }}</p>
				</div>	 
			{% endif %}
		{% endfor %}
		 
		{% endfor %}
	</div>
</div>