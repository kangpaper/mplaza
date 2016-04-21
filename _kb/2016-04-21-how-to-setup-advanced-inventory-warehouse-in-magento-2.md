---
layout: kb
title: "How to Setup Advanced Inventory, Warehouse in Magento 2"
permalink: "/kb/how-to-setup-advanced-inventory-warehouse-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to setup advanced inventory warehouse
---

The Advanced Inventory supports both a short and long configuration form for each product at your store. The configuration form is based on your need of the stock management. Thus, if you find the stock management necessary for your product, let select “Yes” option in the required field and the long form of Advanced Inventory Settings appears. The following guide will help you configure well.

#### Method 1: Exclude Stock Management 

* Go to `Product > Catalog`, click on the `Edit` link in the Product Management.
* On the left-panel, `Advanced Settings > Advanced Inventory`.
* Leave the `Use Config Settings`checkbox empty to make the `Manage Stock` available.  Choose **No** in the field.
* Ehter the number of the Minimum and Maximum Qty Allowed in Shopping Cart in the correspoding field.
* In the `Enable Qty Increment` field, choose **Yes** if you need, then enter the number of items for the incremal sale. Suppose that you offer the number 4, the required quantities in cart is 4, 8, or 16. 
* Hit the `Save`button to finish.

![advanced-inventory-short-form](https://lh3.googleusercontent.com/ijDkirqx4cRMasYGgui3B3E7f7wGvSghxYw8y4pN4w9ZvqznRSICwl6bDkA2ecgIyVqLUJJsA_Tz-1YpMekTYahjgNiPMCYuJxkm3bMTGjioO_MEGqEBtJBTrNMOy5cmEvQgwQVC)

#### Method 2: Inclucde Stock Management

* Go to `Product > Catalog`, click on the `Edit` link in the Product Management.
* On the left-panel, `Advanced Settings > Advanced Inventory`.
* Leave the `Use Config Settings`checkbox empty to make the `Manage Stock` available.  Choose **Yes** in the field.
  * Enter the number of the products in stock in the `Qty` field.
  * Enter the number of the products out of stock in the `Out-of-Stock Threshold` field.
  * Ehter the number of the Minimum and Maximum Qty Allowed in Shopping Cart in the correspoding field.
* In the `Qty Uses Decimals` field, choose **Yes** if the quantity of your products maybe a decimal number. Then, choose **Yes** in the `Multiple Boxes for Shipping` field if you allow dividing the deliveried products into many boxes.
* Consider the `Backorders` from CMS Block: No Backorder, Allow Qty Below 0, or Allow Qty Below 0 and Notify Customer.
* In the `Notify for Quantity Below` field, enter the number of the level that need to notify for the Quantity Below.
* In the `Enable Qty Increment` field, choose **Yes** if you need, then enter the number of items for the incremal sale. Suppose that you offer the number 4, the required quantities in cart is 4, 8, or 16. 
* Choose **In Stock** in the `Stock Availability` field if the product is available in stock.
* Hit the `Save` button to finish.

![advanced-inventory-long-form](https://lh3.googleusercontent.com/2YLviveYWBQP8h6gS0mfoYbP_pbrCTSyF31ei7PqjViXn2BCbpmBT7BMi-AyhbfjCWzt9xR1njyPwPaubLMzLxX48Nyfj3DZ8fEgJzDBiz9a49H5fv4hZu2x6q-igpIZYUJcNhHU)
