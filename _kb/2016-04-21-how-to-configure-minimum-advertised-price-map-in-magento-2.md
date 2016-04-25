---
layout: kb
title: "How to Configure Minimum Advertised Price (MAP) in Magento 2"
permalink: "/kb/how-to-configure-minimum-advertised-price-map-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to configure minimum advertised price MAP
---

In the business, the manufacturers always gives pricing rules that you are compulsory to obey. You can not issue the product with the lower price than the minimum price they offer and allow you to show on the screen. Therefore, to help you provide the best price for the customer, **configuring Minimum Advertised Price (MAP) in Magento 2** is an awesome method for every shop owners.

With **Minimum Advertised Price configuration**, not only you can continue to comply with the producer’s needs but you also have a chance to publish the greater price to your clients. Awaring that the requests are different by many producers, but it is possible for you to set the appearance of your real price on the pages which are not banned by the producers.

Let follow the guides below to become the better providers in the competitive marketplace.

## How to configure Minimum Advertised Price (MAP) in Magento 2

### MAP Logic

Depending on the price of the product to apply the relevant MAP Logic.
* For the price that is set by multiple options,
  * MAP is assigned to the main price while the price of options, bundle items or related items still appear as normal.
  * If the main price is not available, MAP is the price of the related product that maybe in a grouped product. 
  * If a product is in the cart where appears the Manufacturer's Suggested Retail Price, MAP is not deleted.
* For other price configuration,
  * If a tier pricing is set, the tier price appears according to the Display Actual Price setting. 
  * If a special price is set, it is considered to be the actual price for MAP. 

In the order and customer management tools and the reports sections, only the actual price is allowed to present.

### Setup the Minimum Advertised Price (MAP)

You can set the Minimum Advertised Price for all your current products or a single product and the price is still hidden in the store view. Let learn various MAP settings that help your customers shop at your store with the better price while you are well-observed person according to the clause of the producer.

![How to Configure Minimum Advertised Price (MAP) click for price]({{ site.url }}/assets/img/kb/how-to-configure-minimum-advertised-price-map-in-magento-2-click-for-price.png)

You can set MAP configuration for all your products or any specific item as you need. When MAP is used, you need to determine where the actual price appears, simultaneously, edit the explanation message about the hiding of the actual price behind the “Click for price” and “What’s this?” link.  

![How to Configure Minimum Advertised Price (MAP) what's this]({{ site.url }}/assets/img/kb/how-to-configure-minimum-advertised-price-map-in-magento-2-what-'s-this.png)

* Go to the Admin Panel, `Stores > Settings > Configuration`.
* On the left-panel, `Sales > Sales`.
* Click on the `Minimum Advertised Price` section.
* Choose **Yes** in the `Enable MAP` field.

![How to Configure Minimum Advertised Price (MAP) MAP settings]({{ site.url }}/assets/img/kb/how-to-configure-minimum-advertised-price-map-in-magento-2-MAP-settings.png)

#### Method 1: Apply MAP for all your products
* To make the actual price visible to shoppers, choose **On Gesture**, **In Cart** or **Before Order Confirmation** in the `Display Actual Price` field.
* Write the `Default Popup Text Message` in the required box.
* Write the clear explanation about the phrase "What's this?" in the `Default "What's This" Text Message`.
* Hit the `Save Config` button to finish.

#### Method 2: Set up MAP for one product
* On the Admin Panel, `Product > Inventory > Catalog`.
* Click on `Edit` link in the Product Management.
* In the Basic Settings panel, `Advanced Settings > Advanced Pricing`. 

![How to Configure Minimum Advertised Price (MAP) MSRP]({{ site.url }}/assets/img/kb/how-to-configure-minimum-advertised-price-map-in-magento-2-MSRP.png)

  * Import the number of the `Manufacturer's Suggested Retail Price`.
  * Choose the `Display Actual Price` by CMS Block.
    * **Use config** - Use the MAP settings
    * **On Gesture** - Allow showing the actual price after clicking on the **Click for price** or **What's this?** link. 
    * **In Cart** - Show the actual price in the shopping cart.
    * **Before Order Confirmation** - Show the actual price after finishing the checkout process and before confirming the order.
  * Hit the `Save` to finish.
