---
layout: kb
title: How to upload logo in Magento 2
permalink: /kb/how-upload-logo-magento-2.html
published: true
categories: magento-2 magento-2-tutorial magento-2-manage-store magento-2-user-guide
tags: magento-2 how-to manage store logo
---


One of the first things you’ll want to do is to change the logo in the header, and upload a
favicon for the browser. You’ll also want to update the copyright notice in the footer,.
These are a few simple design tasks that you can take care of right away. While your store
is in development, you can turn on the store demo notice, and then remove it when you’re
ready to launch.



## Uploading Your Logo

The size and location of the logo in the header is determined by the store’s theme. Your logo can be saved as either a GIF, PNG, JPG, or SVG file type, and uploaded from the Admin of your store. The default Magento logo in the sample data is an SVG file, which is a scalable XML-based vector graphic format.

![magento 2 upload logo](https://lh5.googleusercontent.com/F82X7Z8sEpG4Oz_WLvtVSJesPzIf4kAJCISXuifsUyS4gdLBvWX3ac8ej6sUbb9IYn0eN3u14WnlT8ppSanAmfIMwjtRDUyEGarZgtPwZc1VJjgf3D_yhniylYAXwDWRgoTGwRiV)

The logo image resides in the following location on the server. Any image file with by that
name and at that location is used as the theme logo.

Path: `app/design/frontend/[vendor]/[theme]/web/images/logo.svg`


If you don’t know the size of the logo, or any other image that is used in your theme, open the
page in a browser, right-click the image, and inspect the element.


In addition to the logo in `the header`, your logo also appears on `email templates` and on `PDF invoices` and other `sales documents`. The logos used for email templates and invoices have different size requirements, and must be uploaded separately

## How to upload frontend logo in Magneto 2

* On the Admin sidebar, tap `Stores`. Then under `Settings`, choose `Configuration`.
* In the panel on the left under `General` choose Design.
* If you have multiple stores or views, set `Store View` in the upper-left corner to the view where
the configuration applies. Then, clear the checkbox after each field so new values can be
entered.
* Expand the `Header` section. Then, do the following:

![upload logo](https://lh4.googleusercontent.com/xwxKv8hQz-2GNtjT4F7Xt70K8D2bmbb5SAx4yMFt4oRQGSyWt0amQB6CPhVd1UjOBCA3ApZCz47VMIpapKBDqQJMnKf9Wpn9x0kyb8Lipgw-J_w4LaegHNdHNdqmH7DOaPqrDRWl)
	
	* To upload a new logo, tap Choose File. Then, choose the file from your computer.
	* Enter the `Logo Image Width` and `Logo Image Height`.
	* In the `Logo Image Alt` field, enter the text that you want to appear when someone hovers
over the image.

* When complete, click `Save Config`


Ref: Magento 2 User Guide