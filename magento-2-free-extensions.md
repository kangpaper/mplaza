---
layout: page
title: Magento 2 Free Extensions
description: "List of all Magento 2 extensions that people love"
permalink:  "/magento-2-free-extensions/"
---

<div class="container">

	<div class="row previews">
		{% for post in site.magento2 %}
            {% if post.price == 0 %}
        		<div class="col-lg-4 col-sm-6">
                    <div class="thumbnail">
                        <a href="{{ site.url }}{{ post.url }}" class="post-image-link">
                            <img src="{{ site.url }}{{ post.image }}" alt="{{ post.title }}">
                        </a>
                        <div class="caption">
                             <a href="{{ site.url }}{{ post.url }}"><h4>{{ post.title }}</h4></a>
                             <p>{{ post.description }}</p>
                            <p>
                                <button type="button" class="btn btn-primary">{% if post.price == 0 %}FREE{% else %} ${{ post.price }}{% endif %}</button>
                                <a href="{{ site.url }}{{ post.url }}" class="btn btn-default">View details</a>
                            </p>
                        </div>
                    </div>
                </div>  
            {% endif %}
		{% endfor %}
	</div>




</div>