---
layout: kb
title: How To Stop Brute Force Attacks in Magento 1, 2
permalink: /kb/how-to-stop-brute-force-attacks-magento.html
published: true
categories: magento-2 magento-2-tutorial magento-2-user-guide
tags: magento brute-force security
---

Brute-force attacks are becoming very common these days. Most websites are by default vulnerable to such attacks. 
If you use Magento, there are by default located at /admin and /downloader and can be abused in several ways. Hackers can easily find them and launch a brute-force attack. In such an attack, random passwords are tried automatically, until one succeeds.

A brute-force attack is one of the simplest methods to gain access to a website because other than patience it does not require any additional skill or resources. Brute-force attacks are simply trial and error. During such an attack, certain permutations and combinations of usernames and passwords are used by hackers to attempt to break into an account.

What should I do?

We are recommend the following best practices

Custom admin path
----------------------

The default Magento 1 backend url is `your-domain.com/admin` Because the default Magento backend URL is common knowledge in brute-force suites, you can easily get some advantage by cutting the low-hanging fruit.

Custom your current admin path as the following:

Edit file `/app/etc/local.xml`
XML Path: `admin -> routers -> adminhml -> args -> frontName`

You can see `<![CDATA[admin]]>`, now change it to your own admin url, e.g: secret or mybackend

Now flush Magento cache to take effect: `System -> Cache Management -> Flush Magento Cache`

*Magento 2*: Not required.

Secure your Magento admin account
-----------------------------------

Don't use admin account
```````````````````````````

People usally use `admin` as first admin account. This is security issue for your Magento store. Because hackers can guest it easily. We recommend you should change `admin` account name to your own account name, nickname or your email address.

Keep strong password
```````````````````````

The best way to protect your Magento store against a brute-force attack is to – and advise other administrators to – use a strong password. 
The rule:

- Password lenght: > 8
- Includes number
- Includes chracters (Lowercase and Uppercase  Characters)
- Include Symbols: optional






