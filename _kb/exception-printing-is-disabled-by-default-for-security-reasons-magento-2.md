---
layout: kb
title: Exception printing is disabled by default for security reasons Magento 1, 2
permalink: /kb/exception-printing-is-disabled-by-default-for-security-reasons-magento-1-2.html
published: true
categories: magento-2 magento-2-error
tags: magento-2 how-to Exception printing disabled security reasons
---


Your store is running Magento 1 or Magento 2, when installing new extensions, setting configuration or even server memory is overload. 
You may get this error **Exception printing is disabled by default for security reasons.** But you still don't know exactly what kind of problem out there. Follow this guide to show the full message.

## ERROR: There has been an error processing your request

```
There has been an error processing your request
Exception printing is disabled by default for security reasons.
Error log record number: 1234567890
```

## Enable Exception printing in Magento 1

You may rename file `errors/local.xml.sample` to `errors/local.xml`

Then Exception printing is enabled, so you can see trace as the following:

![Exception printing is disabled by default for security reasons Magento 1](https://lh4.googleusercontent.com/CHIly_RTi-Zb8Tp1mCVNetkFFuSPwcVR06k3F3lHKXz0wRjT5pPt4XES5ujgnv_zviV_ncLKCahWsBYIuMx5eNl_hkIHA-p8PH_CW5tnHfXJYUWhIgadW-m8qBsRN-Ga61lxjCIH)



## Enable Exception printing in Magento 2

It is similar to Magento 1 but it is located in different folder `pub/errors`

Rename file `pub/errors/local.xml.sample` to `pub/errors/local.xml`

See trace result

![Exception printing is disabled by default for security reasons Magento 2](https://lh5.googleusercontent.com/sR9TmzlvGERjhAN-fN_wGxIywEN9zHhZq8t45Qk6WjyGv9LikRdfx7BTHQJZSKTca8OQkpmEHa-GGKaCmIh24PfLxUMXrMimzvt3bXd7BQCj2dxy1UMu3hr6pLLplxVsFXtyugkg)

