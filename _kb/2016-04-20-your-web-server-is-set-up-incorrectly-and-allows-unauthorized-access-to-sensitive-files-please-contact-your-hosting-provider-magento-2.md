---
layout: kb
title: Your web server is set up incorrectly and allows unauthorized access to sensitive files. Please contact your hosting provider Magento 2
permalink: /kb/your-web-server-is-set-up-incorrectly-and-allows-unauthorized-access-to-sensitive-files-please-contact-your-hosting-provider-magento-2.html
published: true
categories: magento-2 magento-2-error
tags: magento-2 server web unauthorized access
---


After Install Magento 2 package, you may face with the folder permissions error `Your web server is set up incorrectly and allows unauthorized access to sensitive files. Please contact your hosting provider`. Everytime Magento create a new folder, it will set permission to `770` and may get error in this case. If you change to `755`, it is working normally. So how to resolve this error in Magento 2. In this guide, we will show you how to resolve "Your web server is set up incorrectly and allows unauthorized access to sensitive files" correctly.

In Magento Community forum, there are many people had the same problem. 

When look into Magento 2 Code Core, you can see class `Magento\AdminNotification\Model\System\Message\Security` function `getText()` It return the following message: 

```
Your web server is set up incorrectly and allows unauthorized access to sensitive files. Please contact your hosting provider
```

You also see method `_isFileAccessible` for futher information.

In this investigation, we can say all files, folders in `app/etc/*` is accessable from unauthority visitors such as `app/etc/env.php`  file which contain database information, encrypt key, admin URL and more ...


## How to resolve 

First you need to set the permissions on your magento web server directory so that you 'webuser' are the owner of the files and 'nginx' as the group. To do this, as a user with root privileges issue the command:

``chown -R webuser:nginx /path``

where /path = the root path for your magento installation.


And next

`` find . -type d -exec chmod 770 {} \; && find . -type f -exec chmod 660 {} \; && chmod u+x bin/magento ``

Now when you run the cron make sure you are doing this as the owner of the file system, in this example called 'webuser'.
**Do NOT** run it as root as the files created will have root as the owner.




