---
layout: kb
title: "How to create a new category in Magento 2"
permalink: "/kb/how-to-create-a-new-category-in-magento-2.html"
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to create category catalog
---

The category is shown as a big tree with branches in the lower. Each new category created by store owners will be assigned to a relevant parent category. Any unavailable category is hidden with gray. The position of category can be reordered when you drag, hold and drop it to the new location. Moreover, in the top of each category page, the category is marked by a ID number that is next to the category name.


![How to create a new category category tree]({{ site.url }}/assets/img/kb/how-to-create-a-new-category-in-magento-2-category-tree.png)

## Overview of creating a new category

How to create a new category in Magento 2 as following steps:

- Step 1: Generate a Category
- Step 2: Configure the General Information
- Step 3: Configure the Display Settings

### Step 1: Generate a Category
* On the Admin Panel, `Product > Inventory > Categories`
* In the category tree, assign to the relevant category that is right above the new category. 
  
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

Reference: Magento 2 user guide
