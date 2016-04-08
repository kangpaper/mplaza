---
layout: kb
title: How to setup Locale, State, Country in Magento 2
permalink: /kb/how-setup-locale-state-country-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to setup locale state country
---

# Locale Options

Setup your store information on Locale Options that determines the timezone, your language and the days of  the work week in your area. Besides, others can identify your country, tax rate and guest some needed information related to your locale.

![locale options](https://lh5.googleusercontent.com/UzzWUaAmiqM-XwxGsr62ScC_7ehmq4GFgzk14-RzRqkuA9b04rccN8Bav-m-8E6ZqiQqAVwAnpUbNevZ_abyifxvLS7B4UPGnf9hDXGogFUiRCE3iNpshqBwV5csKCgGGA-9ENWB)

## To set the store locale:

* On the Admin sidebar, tap `Stores`. Then under `Settings`, choose `Configuration`.
* In the panel on the left under `General`, choose `General`.
* Expand the `Locale Options` section.
* Select your `Timezone` from the list. Then, do the following:
  * Set `Locale` to the store language.
  * Set `Weight Unit` to the unit of measurement that is typically used for shipments from your locale.
  * Set `First Day of the Week` to the day that is considered to be the first day of the week in your area.
  * In the `Weekend Days` list, select the days which fall on a weekend in your area. (To select multiple options, hold down the Ctrl  (PC) or Command (Mac) key.)
* When complete, tap `Save Config`.

# State Options 

Standard address format is different for every country, so fulfill the state information is optional. In many countries, the state, province, or region is a required part of a postal address that is used for shipping and billing information, to calculate tax rates, and so on. On state options you can setup state is required for which countries.

![state options](https://lh4.googleusercontent.com/xbXbqujpJJLGyJA5hh0cjveb4NnmXWVGWoGwIA8ktFoP7wMNBF-fq7SdD3YtW8hmRx8EY0ZXYrHm_MJsDY44hAWsfPufsgqqQmRWzobOiKS1ZkGv8D9Z4vrDNJlC4kbFcDwzTmB6)

## To set up the state options:

* On the Admin sidebar, tap `Stores`. Then under `Settings`, choose `Configuration`.
* In the panel on the left under `General`, choose `General`.
* Expand the `State Options` section, and do the following:
  * In the `State is required for` list, select each country where Region/State is a required entry.
  * Set the `Allow to Choose State if It is Optional for Country` field to one of the following:
    * Yes      In countries where the state field is not required, includes the State field as an optional entry.
    * No       In countries where the state field is not required, omits the State field.
* When complete, tap `Save Config`.

# Country Options 

The Country Options determines the country where your business is located, and which countries you accept payment. 

![country options](https://lh4.googleusercontent.com/9dHG8cMTAHQsAnb0GhtEz5sMKu6JaplDTulN2Q2yuIc-L0Jh2Eo9xEUS369t-jyGlFSt8wh_kuF1zxpngfL9tD729oHx3M4kCSt5C-lA1GDTa_iRJ31TQcO-YYgWrsR99Rko8vuk)

## To set the country options for your store:

* On the Admin sidebar, tap `Stores`. Then under `Settings`, choose `Configuration`.
* In the panel on the left under `General`, choose `General`.
* Expand the `Country Options` section, and do the following:
  * Choose the `Default Country` where your business is located.
  * In the `Allow Countries` list, select each country from which you accept orders. By default, all countries in the list are selected. To select multiple countries, hold down the Ctrl (PC) or Command (Mac) key.
  * In the `Zip/Postal Code` is Optional for list, select each country where you conduct  business that does not require a ZIP or postal code to be included as part of the street address.
  * In the `European Union Countries` list, select each country in the EU where you conduct business. By default, all EU countries are selected.
  * In the `Top Destinations` list, select the primary countries that you target for sales.
* When complete, tap `Save Config`.

Ref: Magento 2 user guide
