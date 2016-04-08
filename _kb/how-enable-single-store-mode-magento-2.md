---
layout: kb
title: How to enable Single Store Mode in Magento 2
permalink: /kb/how-enable-single-store-mode-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to configure store email
---

Single-Store mode is disabled as setup default that leads to show a scope indicator whenever each configuration setting. Therefore, let enable single-store mode to simplify the display by turning off all Store View options and scope indicators if your Magento Community 2.0 installation has only a single store and view. Learn how to enable single-store mode simply by following steps:

![single store mode disabled](https://lh5.googleusercontent.com/uCdQvYNW-2w1EsRvG4eCz0QB5pzKFuivY9Zn8_POeK-vp5TH4fU3qQPMPtHKFs_DMkuDWrGRY4cz9HdGbAGYhF7MaNgf2GwrvVkCOHEIZprap6Gll9O3Z-9enkI_haNvAO1SZ-lg)

## To set single store mode:

* On the Admin sidebar, click `Stores`. Then under `Settings`, select `Configuration`.
* In the panel on the left under `General`, select `General`.
* Scroll down to the bottom of the page, and expand the `Single Store Mode` section.
* Set Enable Single Store Mode to “Yes.”
* Click `Save Config`.
* When prompted to refresh the cache, do the following:
  * Click the `Cache Management` link in the system message at the top of the page
  * Mark the `Page Cache` checkbox.
  * With `Actions` set to “Refresh,” click `Submit`.

Ref: Magento 2 user guide
