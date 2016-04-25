---
layout: kb
title: "How to Setup Product Price Email in Magento 2"
permalink: "/kb/how-to-setup-product-price-email-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to setup product price email
---

**Setting up Product Price Email** allows creating a lightly notification about the change of your products. There are two kinds of the product price email from Magento 2: **Price Alert** and **In-Stock Alert**. The alert email will be sent to your customers if they sign up to subscribe your alert. From the settings, you need to select the template and the sender for each email. 

If the price alert is active, customers will see the **Sign up for price alert** message on the product detail page of every products. The customers will be navigated to their account page to complete the subscription procedure. The alert notification is definitely sent if there is a light change of the price or a special offer at this time.

![How to Setup Product Price Email sign up for price alert]({{ site.url }}/assets/img/kb/how-to-setup-product-price-email-in-magento-2-sign-up-for-price-alert.png)

Allowing the in-stock alert means the **Sign up to get notified when this product is back in stock** message is shown on the product detail page of the out-of-stock products. Tap the link to receiving the notification whenever the product com back. 

![How to Setup Product Price Email sign up for in-stock alert]({{ site.url }}/assets/img/kb/how-to-setup-product-price-email-in-magento-2-sign-up-for-in-stock-alert.png)

All of subscribers to your alerts are listed in the Product Alert tab of the Product Information page.

## To create product alert

* On the Admin panel, `Stores > Settings > Configuration`.
* On the left-panel, `Catalog > Catalog`.
* Access the `Product Alert` section,
  * To activate the product alert when there is any change of the price, select **Yes** in the `Allow Alert When Product Price Changes` field.
  * Select the template you want to use for the notification when the product price changes from a dropdown list of the `Price Alert Email Template`.
  * To create a light notification if the product come back to the inventory, select **Yes** in the `Allow Alert Product When Come Back in Stock` field.
  
  ~~~
  Set the Display Out of Stock Products in the Inventory Stock Options to Yes if allow showing the Sign up to get notified when this product is back in stock message for the customers
  ~~~
 
  * Select the template used to notify the come back of the product from a dropdown list of the `Stock Alert Email Template`.
  * Select the sender of the alert email in the `Alert Email Sender` field.
  
  ![How to Setup Product Price Email alert email settings]({{ site.url }}/assets/img/kb/how-to-setup-product-price-email-in-magento-2-alert-email-settings.png)

  * Hit the `Save Config` button to finish.
  
## To run product alert

![How to Setup Product Price Email product alert run settings]({{ site.url }}/assets/img/kb/how-to-setup-product-price-email-in-magento-2-product-alert-run-settings.png)

* On the Admin panel, `Stores > Settings > Configuration`.
* On the left-panel, `Catalog > Catalog`.
* Access the `Product Alert Run Settings` section,
  * To set up the level of the frequency to send the product alert, select `Frequency` from a dropdown list of options: Daily, Weekly, or Monthly.
  * Determine the `Start Time` to send the product alert.
  * Enter email address of the person in the ` Error Email Recipient` field to connect if there is any error.
  * Select the sender of the error email in the `Error Email Sender` field.
  * Select the template for the error message in the `Error Email Template` field.
* Hit the `Save Config` button to finish.


Reference: Magento 2 user guide