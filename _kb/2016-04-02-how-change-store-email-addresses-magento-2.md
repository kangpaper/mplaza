---
layout: kb
title: "How to change Store Email Addresses in Magento 2?"
permalink: /kb/how-change-store-email-addresses-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to configure store email
---


You can have up to five different email addresses to represent distinct functions or departments
for each store or view. In addition to the following predefined email identities, there are two
custom identities that you can set up according to your needs.

- General Contact
- Sales Representative
- Customer Support

Each identity and its associated email address can be associated with specific automated email
messages and appear as the sender of email messages that are sent from your store.

<div itemscope="" itemtype="http://schema.org/Question">
	<h3 itemprop="name description">How to change Store Email Addresses in Magento 2?</h3>
</div>

<div temprop="suggestedAnswer acceptedAnswer" itemscope="" itemtype="http://schema.org/Answer">
	<i itemprop="text">Changing Store Email Addresses is one of important tasks when you start selling on Magento 2. To change store email address you can do the following steps:</i>

	<ul>
		<li>Step 1: Set Up the Email Addresses for Your Domain</li>
		<li>Step 2: Configure the Email Addresses for Your Store</li>
		<li>Step 3: Update the Sales Email Configuration</li>
	</ul>

</div>


## Step 1: Set Up the Email Addresses for Your Domain

Before you can configure email addresses for the store, each must be set up as a valid email
address for your domain. Follow the instructions from your server administrator or email
hosting provider to create each email addresses that is needed.

## Step 2: Configure the Email Addresses for Your Store

- On the Admin sidebar, tap `Stores`. Then under `Settings`, choose `Configuration`.
- In the panel on the left under `General`, choose `Store Email Addresses`.
- Expand the `General Contact` section, and do the following:

![magento 2 store email addresses](https://lh5.googleusercontent.com/YBWoihCHcPJVx4JBgAv1dWpEzhdHwMoz17udL2m2LqnZMLHbl9qQO7Qfp95OyegJ6eAhI6-rlHEiYyYrqFo9tXO7RShV3qelD6x1sberh7e25wUxN31jiwWu20hw9FqZ2aCkCgBf)
	- In the Sender Name field, type the name of the person to appear as the sender of any
email messages that is associated with the General Contact identity.
	- In the Sender Email field, type the associated email address.

- Repeat this process for each store email addresses that you plan to use.

- When complete, click  `Save Config`

## Step 3: Update the Sales Email Configuration

If you use custom email addresses, make sure to update the configuration of any related email
messages, so the correct identity appears as the sender.


- In the panel on the left, under Sales, choose Sales Emails. The page has a separate section for
each of the following:
	- Order and Order Comments
	- Invoice and Invoice Comments
	- Shipment and Shipment Comments
	- Credit Memo and Credit Memo Comments
- Starting with Order, expand the section for each message, and make sure that the correct
sender is selected.


![order email template](https://lh3.googleusercontent.com/ueUWbehCZKxUGW3Q-9OLRSDzevyGqZLauZgU6jKPgb0RQl3c8Q15FIiUfQHh2Kkr_MesoF_wuaL1thYvCa3XucoLCyGkb2JFzIqgBwTKKMpkEiiV1OoyYciCjeaux0qtms3_z2kG)

- When complete, click  `Save Config` .


Ref: Magento 2 user guide


