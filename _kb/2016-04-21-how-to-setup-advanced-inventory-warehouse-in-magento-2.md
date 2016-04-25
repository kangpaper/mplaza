---
layout: kb
title: "How to Setup Advanced Inventory, Warehouse in Magento 2"
permalink: "/kb/how-to-setup-advanced-inventory-warehouse-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to setup advanced inventory warehouse
---

**Setting up Advanced Inventory, Warehouse** will help store owners manage the quantities of multiple products very well. For each product, you will configure the advanced inventory such as the published quantity, the minimum and maximum quantity of the product. 

The Advanced Inventory supports both a short and long configuration form for each product at your store. The configuration form is based on your need of the stock management. Thus, if you find the stock management necessary for your product, let select “Yes” option in the required field and the long form of Advanced Inventory Settings appears. The following guide will help you configure well.

## How to Setup Advanced Inventory, Warehouse in Magento 2

### Method 1: Exclude Stock Management 

* Go to `Product > Catalog`, click on the `Edit` link in the Product Management.
* On the left-panel, `Advanced Settings > Advanced Inventory`.
* Leave the `Use Config Settings`checkbox empty to make the `Manage Stock` available.  Choose **No** in the field.
* Ehter the number of the Minimum and Maximum Qty Allowed in Shopping Cart in the correspoding field.
* In the `Enable Qty Increment` field, choose **Yes** if you need, then enter the number of items for the incremal sale. Suppose that you offer the number 4, the required quantities in cart is 4, 8, or 16. 
* Hit the `Save`button to finish.

![How to Setup Advanced Inventory, Warehouse advanced inventory short form]({{ site.url }}/assets/img/kb/how-to-setup-advanced-inventory-warehouse-in-magento-2-advanced-inventory-short-form.png)

### Method 2: Inclucde Stock Management

* Go to `Product > Catalog`, click on the `Edit` link in the Product Management.
* On the left-panel, `Advanced Settings > Advanced Inventory`.
* Leave the `Use Config Settings`checkbox empty to make the `Manage Stock` available.  Choose **Yes** in the field.
  * Enter the number of the products in stock in the `Qty` field.
  * Enter the number of the products out of stock in the `Out-of-Stock Threshold` field.
  * Ehter the number of the Minimum and Maximum Qty Allowed in Shopping Cart in the correspoding field.
* In the `Qty Uses Decimals` field, choose **Yes** if the quantity of your products maybe a decimal number. Then, choose **Yes** in the `Multiple Boxes for Shipping` field if you allow dividing the deliveried products into many boxes.
* Consider the `Backorders` from CMS Block: 
  * No Backorder - not permit any backorder if product is out of stock
  * Allow Qty Below 0 - permit backorder even the quantity is less than 0
  * Allow Qty Below 0 and Notify Customer - permit backorders even the quantity is less than 0 and notify that customer can still place the order
* In the `Notify for Quantity Below` field, enter the number of the level that need to notify for the Quantity Below.
* In the `Enable Qty Increment` field, choose **Yes** if you need, then enter the number of items for the incremal sale. Suppose that you offer the number 4, the required quantities in cart is 4, 8, or 16. 
* Choose **In Stock** in the `Stock Availability` field if the product is available in stock.
* Hit the `Save` button to finish.

![How to Setup Advanced Inventory, Warehouse advanced inventory long form]({{ site.url }}/assets/img/kb/how-to-setup-advanced-inventory-warehouse-in-magento-2-advanced-inventory-long-form.png)
