---
layout: kb
title: How to upload Product Videos in Magento 2
permalink: /kb/how-to-upload-product-videos-in-magento-2.html
published: false
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to upload product videos
---

Adding a video for a product is a great idea to make your product more lively. To do that, you must get an API Key from your Google account and insert it in the configuration. 

## Process Overview

     Step 1: Get Your YouTube API Key
     Step 2: Configure Magento
     Step 3: Link to the Video

## Step 1: Get Your YouTube API Key
* Log in to your Google account, and visit the [Google Developers Console](https://console.developers.google.com/apis/library). Then, follow these:
  * Under **Use Google APIs**, click `Youtube Data APIs`.
  * In the panel on the left choose `Credentials`, click on `Create Credentials` and choose `API key`.
  * When prompted to create a new key, choose `Server key`. Enter a name for the key and IP address, and tap `Create`.
* After you get the key, copy the key to the clipboard.

## Step 2: Configure Magento
* On the Admin Sidebar, `Stores > Settings > Configuration`.
* In the panel, under `Catalog`, choose `Catalog`.
* Expand the `Product Videos` section, paste **Youtube API key** into the required field.

![add-api-key](https://lh4.googleusercontent.com/dYpCuPgKnGRhIgeZT5EhJm6ATKRJgb-7PgjA0Sft3K5WEL8cqJRpGeY-WPMviLoDkKsvqFQ11qWZFm2WA3YoGcjWEnUMatLM8N65Itl7i1sVsvVn0u3C41kz0PJHfMs_P63zZvAN)

* Click `Save Config`.
* Go to `Cache Management` to refresh the cache.

## Step 3: Link to Video

* From the `Poduct Detail`, tap `Add Video` in the `Images and Videos`.

![add-video](https://lh6.googleusercontent.com/aODfQEX9o0fn9ZMH7_uvCql55UewVOvzPZ1oGv0HyO3XvRqaVL9w01vfISy0MwS3ZfmPADZuYRAeo1Ujn0k5OjCN-s37FKXGo6OQjaFziGD3I_laKOoy8jJN2PPMChDTNBhc7LXl)

* Enter the `URL` of the YouTube or Vimeo video.

In the `URL` field, if you haven't entered Youtube API key yet, the system error message will appear, tap `OK` to continue.

![error-message](https://lh6.googleusercontent.com/PeCngC6esXiLQBQxHudA7fe4yQjSt3BznKU-_-bGO1gxNvgSzGF4irPzflrKr5hNVFM1cZJwyvsD1WdGRC-zwnoh3wFlQZHLZsBJddfFQrY_qpS8RJl2ZnIhlhA1kEe0jO8NR59k)

* Enter the `Title` and `Description` of the video.
* To upload a `Preview Image`, browse to the image and select the file.
* If you prefer to use the video meta data, tap `Get Video Information`.
* To assign the role to the video, mark the corresponding checkbox of each Role:
  * Base Image
  * Small Image
  * Swatch Image
  * Thumbnail
  * Hide from Product Page
* When complete, tap `Save`.

![product-video](https://lh4.googleusercontent.com/NT_GVEeqfHnsyO2sAPP5JcMLUpoopU6kX-2Pic7MqTpZNE0vbcd8H9_VTHLP9aWz0PCFiHonCHdGDlw5hzxzGH9qbEuRmc7oAKDtiYKbsYQk1FMBKjB3LaJj5qL1ARV9_NrK9_kv)
  
  
