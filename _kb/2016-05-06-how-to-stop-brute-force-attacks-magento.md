---
layout: kb
permalink: /kb/how-to-stop-brute-force-attacks-magento.html
published: true
categories: m2 m2-userguide
tags: magento brute-force security
---

Brute-force attacks are becoming very common these days. Most websites are by default vulnerable to such attacks. 
If you use Magento, there are by default located at /admin and /downloader and can be abused in several ways. Hackers can easily find them and launch a brute-force attack. In such an attack, random passwords are tried automatically, until one succeeds.

A brute-force attack is one of the simplest methods to gain access to a website because other than patience it does not require any additional skill or resources. Brute-force attacks are simply trial and error. During such an attack, certain permutations and combinations of usernames and passwords are used by hackers to attempt to break into an account.

What should I do?

We are recommend the following best practices

1. Custom admin url
----------------------

The default Magento 1 backend url is `your-domain.com/admin` Because the default Magento backend URL is common knowledge in brute-force suites, you can easily get some advantage by cutting the low-hanging fruit.

Custom your current admin path as the following:

Edit file `/app/etc/local.xml`
XML Path: `admin -> routers -> adminhml -> args -> frontName`

You can see `<![CDATA[admin]]>`, now change it to your own admin url, e.g: secret or mybackend

Now flush Magento cache to take effect: `System -> Cache Management -> Flush Magento Cache`
