---
layout: kb
title: "How to setup Stock in Magento 2"
permalink: "/kb/how-to-setup-stock-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to setup stock  
---

To make the shopping easier, you can let customers see the availability of the product they are interested in. On the storefront, “In Stock” and “Out of Stock” will describe this availability. 

## Set up the Stock Options

The Stock Options might be active for a entire of the products in the catalog and the quantity in stock is updated continuously. Moreover, the Stock Options help you drive more new clients shopping at your store not just those who buy a huge quantity of the products, you enable to set the maximum for an order instead of taking the whole from your inventory.

* On the Admin panel, `Stores > Settings > Configuration`.
* On the left-panel, `Catalog > Inventory`.
* In the `Stock Options` section, 
  * Select **Yes** in the `Set Items' Status to be In Stock When Order is Cancelled` field when the order is postponed, and the product is given back.
  * Set `Decrease Stock When Order is Placed` to **Yes** as soon as adding or minusing the quantity of the product in the shopping cart.
  * The `Display Out of Stock Products` is Yes if you approve to show the product in the catalog despite of it is no longer in stock.
    
    If need, enable the price alert to notify the comeback of the product in stock for customers who have already logged in to follow that.
  * Enter the number of the product left in stock in the `Display X left Threshold` field. In the Store View, "Only X left" will be shown for the buyers. For example, only 3 left.
  * Make the quantity in stock or out of stock visible on the product detail page if choose **Yes** in the `Display Products Availability In Stock on Storefront`field.
* Hit the `Save Config` button to finish.

![stock-option-config](https://lh6.googleusercontent.com/yKyhze7sc1Rt9_LAQC0ToF2ANaVr_PT7zxIYPsHzy-cL1zPrsciRfe4e3qlSKhjzzrsSbFNGRyLsazaGmBqise1tPehHBLykgQaRXG8AjrfkNROKy2swZwsDSDnmNZvMxXA22Ymf)

## Set the Product Stock Options

The Product Stock Options means the inventory settings at the product level. However, the Product Stock settings only applies for a single product instead of all items in a cart.

* On the Admin panel, `Stores > Settings > Configuration`.
* On the left-panel, `Catalog > Inventory`.
* In the `Product Stock Options` section,
  * To apply the inventory tracking for your product, say **Yes** to `Manage Stock`.

![product-stock-option-config](https://lh5.googleusercontent.com/qHVgd-5kJSF3Oba7hjg5OVqa8LBfsDjrJK3y96B_jUq2AvmMd-UaEXN41tr2-jDk2hvpol_gfYOZGZb_GF3Gv5txtuN0Rl9qDaL9GQU30ueu6ur_kU9InCD-ZVEDfRBLQwoNJDCr)
  
  * Select one of the options for `Backorders:  
    * No Backorder - not permit any backorder if product is out of stock
    * Allow Qty Below 0 - permit backorder even the quantity is less than 0
    * Allow Qty Below 0 and Notify Customer - permit backorders even the quantity is less than 0 and notify that customer can still place the order. 
  * Insert the `Maximum Qty Allowed in Shopping Cart`.
  * Insert the `Qty for Item's Status to Become Out of Stock`.
  * Insert the `Minimum Qty Allowed in Shopping Cart`.
  * Insert the quantity of product in the `Notify for Quantity Below`. For example, if there are 1 item in stock, an alert is on to notify that the item is out of stock.
  * In the `Enable Qty Increment` field, choose **Yes** if you need, then enter the number of items for the incremal sale. Suppose that you offer the number 4, the required quantities in cart is 4, 8, or 16. 
  * Choose **Yes** for `Automatically Return Credit Memo Item to Stock`, that means if there is any problem of the credit memo, the placed item will be back to the inventory.
* Hit the `Save Config` button to finish.

