---
layout: kb
title: "Magento 2 You Don't Have Permission To Access / On This Server"
permalink: /kb/magento-2-you-do-not-have-permission-to-access-on-this-server.html
published: true
categories: magento-2 magento-2-error
tags: magento-2 server web permission access
---

Your store is running Magento 2 and suddently got this error *You don't have permission to access /magento on this server.* You may get crazy with Linux folder permission in this case. No worry, there is a simple solution for that.

This error indicates that a default document could not be found at the specified URL and that directory listings are not permitted.

## Problem

~~~
Forbidden

You don't have permission to access /magento on this server.
~~~


## Solution


Grant permissions

~~~
sudo chown -R $USER:$USER /var/www/magento
sudo chmod -R 755 /var/www
~~~

You can replace correct Magento path `/var/www/magento`

Happy coding!

