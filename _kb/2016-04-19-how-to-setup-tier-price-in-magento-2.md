---
layout: kb
title: "How to Setup Tier Price in Magento 2"
permalink: "/kb/how-to-setup-tier-price-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to setup tier price 
---

With Tier Pricing config, you can give a certain group or store view a special offer that is displayed on both the product list and the product page. 

* On the product list page, the tier price will go together with the words "As low as" as the following:

![tier-pricing-as-low-as](https://lh6.googleusercontent.com/Ehrn9ZovjRV-IBugw-iqBDB6GrDtxtt-j-w5DjobNqxtQulojLP9y-EhBlGsDJb28LO4SLlQJ9haOpblnWWGcmhTNCPK5ylSD8XqiqBlx0eB2BdZtzEs5oMDCAwCMUdbTQIuALp2)

* On the product page, customers will get the discount from a short message:

![tier-pricing-on-product-page](https://lh5.googleusercontent.com/624TxbXhDO5Sx52Y-QZJJDxDxkAsJNQi5GgxyicSL6smWh-6KGfKyjfpjNNUKpbSc-AAVXtVqgvdyQZrohuPVwSvkCsmneFTE52Jt8yuwe3Sijd74--os2M2Zsg_Q_pZMeNydW6q)

## Set up a tier price
* Open the product in edit mode.
* In the basic settings panel, `Advanced Settings > Advanced Pricing`.
* In the Tier Price area, click `Add Tier` and do the following:

![set-up-tier-pricing](https://lh3.googleusercontent.com/H16sEm2hqEQBgHdl-aYYfuvlZ-LAM7CenXVZAmmaIuQG0Yx6Nfd9cTrb0tl1mS33kF5HQpfzmmM2RfAvTZV3A2nk7Vc5fTtLwm51sd3h2FT_aN81Z8wJIvlM8MS-Smbs8i9zEx6x)

  * If you have many websites, choose the `Website` where you want to set the tier pricing.
  * Select the `Customer Group` who receive the discounted price.
  * In the `Quantity` field, enter the required number of product to get the deal.
  * In the `Item Price` field, enter the desired price of the product.
    
    Enable to add as many tiers as you need by clicking on `Add Tier` and repeat these steps. For exxample, you set up 2 tiers for a product while tier 1 requests for 2 products in an order and tier 2 needs for 5 items. If your customer have 4 items in the cart, the offer for tier 1 will apply for that order. Only when the number of product in the cart is 5, the customer will get the discounted price in the tier 2 instead of the discount in the tier 1.

* Hit the `Save` button to finish.
