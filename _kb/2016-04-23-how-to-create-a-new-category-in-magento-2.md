---
layout: kb
title: "How to create a new category in Magento 2"
permalink: "/kb/how-to-create-a-new-category-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to create category catalog
---

**Creating a new category** is the essential way to establish the logic flow for your management in the settings. Besides, customers will find the searching on your website professional instead of making the appearances of all items chaos.
 
The category is shown as a big tree with branches in the lower. Each new category created by store owners will be assigned to a relevant parent category. Any unavailable category is hidden with gray. The position of category can be reordered when you drag, hold and drop it to the new location. Moreover, in the top of each category page, the category is marked by an ID number that is next to the category name.

![How to create a new category category tree]({{ site.url }}/assets/img/kb/how-to-create-a-new-category-in-magento-2-category-tree.png)

In Magento 2, it is possible to create a new category as well as custom it as you expect.

## Overview of creating a new category

How to create a new category in Magento 2 as following steps:

- Step 1: Generate a Category
- Step 2: Configure the General Information
- Step 3: Configure the Display Settings

### Step 1: Generate a Category
* On the Admin Panel, `Product > Inventory > Categories`
* In the category chart, assign to the relevant category that is right above the new category. 
  
  If there is any data which is fit with the new category, you can assign to the **Default Category**.

* Hit the `Add Subcategory`.

### Step 2: Configure the General Information
* On the `General Information` section,
  * Name for the new category.
  * Enable the category by choosing **Yes** for `Is Active` field.
  * Create a `URL Key` for own or it will be auto-created by the system.
* Write some descriptions about the category in the `Desscription` box.
* Upload the `Image` for the category if need.
* Enter the data: `Page Title`, `Meta Keywords`, `Meta Decription` for your SEO.
* In the `Include in Navigation Menu` field, choose **Yes** to show it on the Navigation Menu.
* Hit the `Save Category` button.

### Step 3: Configure the Display Settings

* Consider the `Display Mode` from the following options: Products Only, Static Block Only or Static Block and Products.
* Select a type of the static block in the `CMS Block` to show on the category page.
* `Is Anchor` is your aggrement to show the "Filter by Attributes" of the layered navigaiton. If accept, choose **Yes**.
* If you don't want to use config settings, ignore the checkbox and choose a feature (Name, Price) to reorder a list of product.

![How to create a new category displaying settings]({{ site.url }}/assets/img/kb/how-to-create-a-new-category-in-magento-2-displaying-settings.png)

* Hit the `Save Category` to complete.

## Customizing Categories

A category configuration is customizable, so you can fix, change its position in the category chart, even eliminate it quickly. However, it is important to examine how your modification will affect on other parts. For instance, if there are some products in the category that you rename, the current product links are unavailable to access. Therefore, you should set your catalog to auto-generate a permanent redirect if there is any change as above. Or you can apply the URL Rewrite tool to navigate the visitors to a new link.

### Rearrange a category

* On the Admin Panel, `Product > Inventory > Categories`
* In the category chart, tap the needed category and drag-drop it to the new parent category. The new structure of category will be auto-saved.

### Eliminate a category

* From the category chart, consider the category you want to eliminate. 

~~~
A eliminated category never comeback, so be careful to select the right category.
~~~

* Click on the `Delete Category`, then `Ok` to verify.

Reference: Magento 2 user guide
