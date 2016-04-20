---
layout: kb
title: How To Stop Brute Force Attacks in Magento 1, 2
permalink: /kb/how-to-stop-brute-force-attacks-magento.html
published: true
categories: magento-2 magento-2-tutorial magento-2-user-guide magento
tags: magento brute-force security
---

Brute-force attacks are becoming very common these days. Most websites are by default vulnerable to such attacks. 
If you use Magento, there are by default located at /admin and /downloader and can be abused in several ways. Hackers can easily find them and launch a brute-force attack. In such an attack, random passwords are tried automatically, until one succeeds.

A brute-force attack is one of the simplest methods to gain access to a website because other than patience it does not require any additional skill or resources. Brute-force attacks are simply trial and error. During such an attack, certain permutations and combinations of usernames and passwords are used by hackers to attempt to break into an account.

What should I do?

We are recommend the following best practices

## Custom admin path


The default Magento 1 backend url is `your-domain.com/admin` Because the default Magento backend URL is common knowledge in brute-force suites, you can easily get some advantage by cutting the low-hanging fruit.

Custom your current admin path as the following:

Edit file `/app/etc/local.xml`
XML Path: `admin -> routers -> adminhml -> args -> frontName`

You can see `<![CDATA[admin]]>`, now change it to your own admin url, e.g: secret or mybackend

Now flush Magento cache to take effect: `System -> Cache Management -> Flush Magento Cache`

*Magento 2*: Not required.

## Secure your Magento admin account


### Don't use admin account


People usally use `admin` as first admin account. This is security issue for your Magento store. Because hackers can guest it easily. We recommend you should change `admin` account name to your own account name, nickname or your email address.

### Keep strong password


The best way to protect your Magento store against a brute-force attack is to – and advise other administrators to – use a strong password. 
The rule:

- Password lenght: > 8
- Includes number
- Includes chracters (Lowercase and Uppercase  Characters)
- Include Symbols: optional



## Protect /downloader folder

In Magento 1, it use `/downloader` called **Magento Connect Manager** folder to install extension from Magento Connect. This is default path, it is easy for hacker to attack your Magento website. You can rename it but there is a effect way to protect the `downloader` folder, it is *IP whitelist*


### Apache
Edit file `downloader/.htaccess` and add the folowing lines to the end:

```xml
order deny,allow
deny from all
allow from x.x.x.x
```
x.x.x.x is your whitelist IP v4 address.


### Nginx

Open configuration file of your Magento website.
E.g: `/etc/nginx/conf/mywebsite.conf`

Add the following block of lines:

```xml
location /downloader/ {
  allow x.x.x.x;
  deny all;

  location ~ \.php$ {
    echo_exec @phpfpm;
  }
}
```


### Cpanel or DA hosting

You can ask for support from your hosting providers.


## Protect local.xml file

`local.xml` file is very sensitive data that contain database information, admin path or crypt key.
If this information is leak to public you will get problem.

Check it now, navigate your browser to `http://your-domain.com/app/etc/local.xml`
If it cannot access to the data, your website is safe. Otherwhile, you can follow the `Protect /downloader folder` in previously to disable that.


## Secure .git folder

Git is now popular nowsday, every store using Git as version control of its store. Git folder contain many important information such as repo url, code files ...

You can follow the `Protect /downloader folder` in previously to disable that.


## Is your store up-to-date?

- Apply security paches. There are some security patches that Magento released recently, you can download it at (here)[https://www.magentocommerce.com/download]
- Install Magento latest version. Updating to latest version that keep your store always healthy.


## Enable HTTPS for admin panel

Since Magento is used for e-commerce transactions, the data is often very sensitive. This is why it is recommended that all of your login details should pass through a secure connection.

Go to `System > Configuration > Website`

![enable ssl in magento admin](https://lh4.googleusercontent.com/rzWqHt4yibZFIyysSpBgT-xrHUbP4n-QdH5HCgekCqVqwe35ZQOTfeHBoZky9ZATV8n0a8HM7PvpxLPnHZYhfaa8Wrqw-qfsZo3KvIghA3N_xBPjxHH5EuwDjp2E6tygHt7PK6Hl)



```php

<?php

echo 'Magento';

Mage::getModel('catalog/product')->getCollection();

?>
```