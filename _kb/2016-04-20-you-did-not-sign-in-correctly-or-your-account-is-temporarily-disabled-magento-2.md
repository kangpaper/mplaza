---
layout: kb
title: You Did not Sign in Correctly or Your Account is Temporarily Disabled Magento 2
permalink: /kb/you-did-not-sign-in-correctly-or-your-account-is-temporarily-disabled-magento-2.html
published: true
categories: magento-2 magento-2-error
tags: magento-2 how-to account disabled
---

When you try to login to your Magento admin, you got this message ``You did not sign in correctly or your account is temporarily disabled`` . You don't know that you are not using username or password. In this guide, we will show to how to resolve this sign in problem "You did not sign in correctly or your account is temporarily disabled".

In Magento forum, you can see there are many people had same problem.

![You did not sign in correctly or your account is temporarily disabled](https://lh4.googleusercontent.com/MxzGBZWUuJL1-8cZdlv8jP4pUvsGOQ0gbWAaVcrM-B-NHnJ31UDOp7e5mHFyL2Z0p-L4AJlxy-spME255OzZVu2tqPPqZy8cTvBy_wXu5cSFvX1V0UQiaiAc_KXYGsDBx6RYiPRn)



## You did not sign in correctly or your account is temporarily disabled.


I have been installing via the command line and ran into this problem yesterday, after banging my head off the wall all day, I tried creating a new user via the cli ``./bin/magento admin:user:create`` and that’s when I noticed an error. I guess usually my random typing contains numbers.

The fix was to make sure there is 1 alpha character and 1 numeric character in the admin password. This should be labelled a bug if the password is not validated during install with ``magento setup:install``


### Password requirements are:

- User Name is a required field.
- First Name is a required field.
- Last Name is a required field.
- Please enter a valid email.
- Password is required field.
- Your password must be at least 7 characters.
- Your password must include both numeric and alphabetic characters.

Reference: `@rapidmod`

## Unlock admin account

try command in case the account is locked

~~~
./bin/magento admin:user:unlock <username>
~~~
