---
layout: page
title: Sitemap
permalink:  "/sitemap/"

---

Sitemap
---------



<h2>Magento extensions</h2>

<ul>
{% for post in site.magento-extensions %}
<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>



<h2>Magento 2 extensions</h2>

<ul>
{% for post in site.magento2 %}
<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>



<h2>Knowledge base</h2>

<ul>
{% for post in site.kb %}
<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>






<h2>Blog posts</h2>

<ul>
{% for post in site.posts%}
<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
