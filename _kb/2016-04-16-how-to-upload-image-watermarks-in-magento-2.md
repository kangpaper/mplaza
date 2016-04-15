---
layout: kb
title: How to upload Images Watermarks in Magento 2
permalink: /kb/how-to-upload-image-watermarks-in-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to upload images watermarks
---

If you don’t want anyone to use your original product image that you have already published, set the image watermarks for each image to identify them as yours. Many types of image are supported here as .jpg (jpeg), .gif, or .png image. An example for the image watermark settings:

* Size: 200x300 
* Opacity: 40
* Position: Stretch

![stretch-watermark](https://lh3.googleusercontent.com/IRbVFS1fNGG1omUiGrZnJ8uSEOFQwZBc1HK2bkRBEe3F_y7xi68ypP5p8aAJFwW3pHJ2KlJvl0Et-qAiXG05wfF00R21MWDDX5Vb8Wl5QlAfI9n-QQk1YjpD8vqbf6PYI0r9AEtj)

## Process Overview

     Add watermark to product images
     Delete a watermark

## Add watermark to product images
* On the Admin sidebar, `Stores > Settings > Configuration`.
* In the panel, `General > Design`.
* Expand the `Product Image Watermarks` section and complete the following steps for the Base, Small, and Thumbnail images:
  * Enter the `Watermark Default Size` in pixels.
  * Enter the `Watermark Opacity`, `Percent` as a percentage.
  * Tap `Choose File`, to upload the image file.
  * Set `Watermark Position` to your preference.

![product0-watermark-config](https://lh3.googleusercontent.com/3obnVxPKHKRapc--IM9PtNpuIIFC3FkAwwWRVcnbTlOf4HUAPe7oCH_oraiSwelluoflCRH9zGmy7XLXpe_lstk6bthqf7f3GtXO1dK_FMlvnirNrxP3OYij1w-YqKuej2cHsNeQ)

* When complete, tap `Save`.
* Go to `Cache Management` to refresh the cache.

## Delete Watermark

* Mark the `Delete Image` checkbox to delete a watermark.

![delete-watermark](https://lh4.googleusercontent.com/zJ0ZvRRlj2ofzcgtKq9y_pjRhdMqAMEI1xU08gAi796uVpSjzRdTVOOSOlDVLrID23rjaAKALRB1wLwIma4309dIhwfGAnTmaI2X4EHzaKsXGBU8cagjM2C6iPGD80N7zgu2xwK0)

* When complete, tap `Save Config `.
* Go to `Cache Management` to refresh the cache.
