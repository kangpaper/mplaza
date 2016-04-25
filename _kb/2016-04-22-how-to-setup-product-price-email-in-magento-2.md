---
layout: kb
title: "How to Setup Product Price Email in Magento 2"
permalink: "/kb/how-to-setup-product-price-email-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to setup product price email
---

There are two kinds of the product price email from Magento 2: **Price Alert** and **In-Stock Alert**. The alert email will be sent to your customers if they sign up to subscribe your alert. From the settings, you need to select the template and the sender for each email. 

If the price alert is active, customers will see the **Sign up for price alert** message on the product detail page of every products. The customers will be navigated to their account page to complete the subscription procedure. The alert notification is definitely sent if there is a light change of the price or a special offer at this time.

![sign-up-for-price-alert](https://lh5.googleusercontent.com/yilGF4RxfkE_zXJ_8R1BKZbbPAKuu_pzQ5ELAJZRMx6PyJe3oi6kASWUGcooho7kSQuuyrZT7-laKhTC_3qDNtSzLo7TaLdhJUop6pCmhmJtuVvd3lqhuRnf26N3RD-kVT8MqKTU)

Allowing the in-stock alert means the **Sign up to get notified when this product is back in stock** message is shown on the product detail page of the out-of-stock products. Tap the link to receiving the notification whenever the product com back. 

![sign-up-for-in-stock-product](https://lh4.googleusercontent.com/nsvzc91j0hvbJ-AMtg0rXrXgtBQJ5i9HHsJx1i8nHNhR-igWENj56Y7anPFBBt_uyQIbG0CoscbG_GJP4I72DH9lep9DDxXn8zL4c_yzA8rZdbkuMLsIsBYKcdVIwU9bXpqexDWE)

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
  
  ![alert-email-settings](https://lh6.googleusercontent.com/gwmwJFWnVmL3yHeVunDe_zFcHj9-MBgu_o2_I2VfBfvqxLpCephTcMBxX_BOq1FwN8H2MsQUreADEbhnICoiA7JQJCm_SJ_AdUnn5SjeUM7ygSwC9fLkpCG9-DGUOoAMsGv3TYXs)
  
  * Hit the `Save Config` button to finish.
  
## To run product alert

![product-alert-run-settings](https://lh4.googleusercontent.com/i2D6MSK45jX_oYPuk8Tu6TWVjtHrU4VRV-Z51MDweG6dWNnz5kPHzHK07taBcExKUJ_ewFXpEExQTJcOZgChD55H8sJ-xloq8zeCkC24C5fS64cy1iHMiugcG4S6_jLWGrX-anAS)

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