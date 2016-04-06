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

![enable contact us form](https://lh4.googleusercontent.com/O0bmPb6nqTYsMPlmvM6g9RT4kSgYazcwfzKz18i7hXwiELUmpcotbPawYNTo30QBG9OmGY_W7qTIBPkFng8KxJgd0fGgmU0WjTlX2yVbxv6Vlxf7hG56YhH7A_Lr4SkVOyqGSIiw)

* Expand the `Email Options` section. Then, do the following:
	* In the `Send Emails` to field, enter the email address where messages from the `Contact Us` form are sent.
	* Set `Email Sender` to the store identity that appears as the sender of the message from the Contact Us form. For example: Custom Email 2.
	* Set Email Template to the template that is used for messages sent from the Contact Us
form.


![email options](https://lh5.googleusercontent.com/J2S2OY8vAaM9SoAW3jdqhqF2NVJTSbYHoqWHWKE-79N8RWSZ0aPusaj5_yXjFamtMWHQBGBZ4RGEdem5WYv10AsaevpX0e-nQamdZgJU-rC8DXHw6gi5FjP57qLElAy2Pzy6oR3P)


When compete, click `Save Config`.



## To customize the Contact Us form:

* On the Admin sidebar, tap Content. Then under Elements, choose Blocks.
* Find the Contact Us Info block in the list, and open in Edit mode.

![contact us in block](https://lh5.googleusercontent.com/mdZFQ3iAmQaRqlasp60-Ic3rzJ-E02LpO-H-XOfo6xUk7UK-ZhiZ49XeathgG01kh1MzTSV5XAoKOEJSWEubcM3WKtIJXSUcCMAczgHwVXN6Nu0a2fAHnLxNbo6xchrMrMpSVba3)

* Scroll down to the `Content` field, and make any changes necessary.
	* Use the editor toolbar to format the text, and add images and links.
	* Click on `Show / Hide Editor` to work directly with the HTML.

![Edit contact us information](https://lh6.googleusercontent.com/3ZCaJ4igseCgojqU7uivRiTNRphyYH1Uhsw9estfqibug1YgXmfrTGjXa2VVDGAm83pFM31CGzATWZi-gTTyVUczmMf1qzRxiyRWG387GFVgg65hDU746sq9tT_DFlN_n5WWVYn-)

* When complete, Click on `Save Block`
