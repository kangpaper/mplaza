---
layout: kb
title: How to configure Contacts form and contact email address in Magento 2
permalink: /kb/how-configure-contacts-email-address-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to configure email contacts
---

The Contact Us link in the footer of the store is an easy way for customers to keep in touch with
you. Customers can complete the form to send a message to your store.

By default, Magento setup email address is `hello@example.com` now you have to change to your own email address.
You also can custom email template of contact message.

Here are Contact us form in frontend, visitors/customers can send you an email via this page.

![magento 2 contact us form](https://lh3.googleusercontent.com/M6ykx1oP09jJLujtv1FGxLziTJsQpwX_Lzspz79WtvCM3gzwS5CDm7VZXQlS4bbjqCLVhBZxfysGDd1ZfunQtLvLGzjoVpM6LjFFo-jkwZTwRP7cPuUKghesDd95UuTR6SquwhIe)


After the form is submitted, a thank you message appears. The contact-us-info block
contains the form, and can be easily customized.


## How to configure Contact Us form

* On the Admin sidebar, click `Stores`. Then under `Settings`, choose `Configuration`.
* In the panel on the left under `General`, choose `Contacts`.
* Expand the `Contact Us `section. If necessary, set `Enable Contact Us` to “Yes.”

img 1

* Expand the `Email Options` section. Then, do the following:

..* In the Send Emails to field, enter the email address where messages from the Contact Us form are sent.
..* Set Email Sender to the store identity that appears as the sender of the message from the Contact Us form. For example: Custom Email 2.
..* Set Email Template to the template that is used for messages sent from the Contact Us
form.


img 2