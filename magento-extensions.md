---
layout: page
title: All Extensions
description: "Magento Extensions"
meta-title: "The Best Magento Extensions"
meta-description: "Best Magento Extensions"
permalink:  "/magento-extensions/"
redirect_from:
  - /categories/extension/
  - /categories/extensions/
---

<div class="container">
	<div class="row previews">
		{% for post in site.magento-extensions %}
		<div class="col-lg-4 col-sm-6">
            <div class="thumbnail">
                <a href="{{ site.url }}{{ post.url }}" class="post-image-link">
                    <img src="{{ site.url }}{{ post.image }}" alt="{{ post.description }}">
                </a>
                <div class="caption">
                    <h4>{{ post.title }}</h4>

                    <p>
                        <button type="button" class="btn btn-primary">{% if post.price == 0 %}FREE{% else %} ${{ post.price }}{% endif %}</button>
                        <a href="{{ site.url }}{{ post.url }}" class="btn btn-default">View details</a>
                    </p>
                </div>
            </div>
        </div>
		{% endfor %}
	</div>
</div>