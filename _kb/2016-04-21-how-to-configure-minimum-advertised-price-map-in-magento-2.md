---
layout: kb
title: "How to Configure Minimum Advertised Price (MAP) in Magento 2"
permalink: "/kb/how-to-configure-minimum-advertised-price-map-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to configure minimum advertised price map
---

In the business, it is intelligibility when the merchants are not allowed to give a lower price than that the manufacturer offer. However, with Minimum Advertised Price from Magento, not only you can continue to comply with the producer’s needs but you also have a chance to publish the greater price to your clients. Awaring that the requests are different by many producers, but it is possible for you to set the appearance of your real price on the pages which are not banned by the producers.

## MAP Logic

Depending on the price of the product to apply the relevant MAP Logic.
* For the price that is set by multiple options,
  * MAP is assigned to the main price while the price of options, bundle items or related items still appear as normal.
  * If the main price is not available, MAP is the price of the related product that maybe in a grouped product. 
  * If a product is in the cart where appears the Manufacturer's Suggested Retail Price, MAP is not deleted.
* For other price configuration,
  * If a tier pricing is set, the tier price appears according to the Display Actual Price setting. 
  * If a special price is set, it is considered to be the actual price for MAP. 

In the order and customer management tools and the reports sections, only the actual price is allowed to present.

## Setup the Minimum Advertised Price (MAP)

You can set the Minimum Advertised Price for all your current products or a single product and the price is still hidden in the store view. Let learn various MAP settings that help your customers shop at your store with the better price while you are well-observed person according to the clause of the producer.

![click-for-price](https://lh5.googleusercontent.com/a0-LzUx8Fo0HBW_fqvTEL26hR0V5kPn-6db3D6pJD7w2lMBBinijxXT1eiEl9SYcvUhUJ0PqQPx376502fhlCXyJyx6EOe26yptWSfRPQ9razxgLa73eQmsSlI601XOeT2aYxYOK)

You can set MAP configuration for all your products or any specific item as you need. When MAP is used, you need to determine where the actual price appears, simultaneously, edit the explanation message about the hiding of the actual price behind the “Click for price” and “What’s this?” link.  

![what-'s-this](https://lh5.googleusercontent.com/_cqe29ciYsxHSUsIh8f9h81PN9JsJ_E1sRcSdoqS-zwMiySrXUL88CLH1gu5ZqKjYqXOPyU9XmaAoPhpcBWEd4E1usYdUI8dLO44bHG7BGoqIGlHpYd_Rs15WG4sa4rObBUIRXTQ)

### To set up MAP
* Go to the Admin Panel, `Stores > Settings > Configuration`.
* On the left-panel, `Sales > Sales`.
* Click on the `Minimum Advertised Price` section.
* Choose **Yes** in the `Enable MAP` field.

![map-settings](https://lh4.googleusercontent.com/NBoowl7JoqPDTsIkzwd6ZvtA2Q7eSDIpWoSHZQ4YZA4u4mJMYbUQ8xdB3U-BtM5v-9TeiWe9uROcqnyf6z_Ls69pBGWD-1Xay4musE7K8mAYUeEbbj4hNZuyMjOdU7YQMVsKTA-f)

#### Method 1: Apply MAP for all your products
* To make the actual price visible to shoppers, choose **On Gesture**, **In Cart** or **Before Order Confirmation** in the `Display Actual Price` field.
* Write the `Default Popup Text Message` in the required box.
* Write the clear explanation about the phrase "What's this?" in the `Default "What's This" Text Message`.
* Hit the `Save Config` button to finish.

#### Method 2: Set up MAP for one product
* On the Admin Panel, `Product > Inventory > Catalog`.
* Click on `Edit` link in the Product Management.
* In the Basic Settings panel, `Advanced Settings > Advanced Pricing`. 

![MSRP](https://lh4.googleusercontent.com/wB20jsdRpDpsM1p7blORdoDCzGuB_vGn0HT5eEh1MfKTEPIuKcbrrby9_rnhSzJKlvM6ZofXQ9NMY9RBhlKXDnGolM_CKnz3l81nkojBWfa9R4OKnzdmTEtCgRzVaV-jFPkDh487)

  * Import the number of the `Manufacturer's Suggested Retail Price`.
  * Choose the `Display Actual Price` by CMS Block.
    * **Use config** - Use the MAP settings
    * **On Gesture** - Allow showing the actual price after clicking on the **Click for price** or **What's this?** link. 
    * **In Cart** - Show the actual price in the shopping cart.
    * **Before Order Confirmation** - Show the actual price after finishing the checkout process and before confirming the order.
  * Hit the `Save` to finish.
