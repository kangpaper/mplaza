---
layout: kb
title: "Magento 2 Layout, Block & Template Ultimate Guides"
permalink: /kb/magento-2-layout-block-template.html
published: true
categories: magento-2 magento-2-tutorial magento-2-frontend
tags: magento-2 how-to block template layout
---


Carrying on from our previous overviews of the main changes for front-end developers in Magento 2, we’ll now look specifically at the revisions to the templating system. While the changes aren’t too drastic, developers will want to become familiar with the new system - particularly those upgrading sites from Magento 1.x to Magento 2. This guide will take developers through the changes to layout XML and the new overall project structure of Magento 2


One of the biggest differences between the two versions of Magento is the way
the whole project is structured. Unlike Magento 1.x where templates were defined
in `app/design/frontend/<package>/<your_theme>` and your theme assets
defined in `skin/frontend/<package>/<your_theme>`, in Magento 2 everything is
consolidated into one base folder location. In this case, there is no longer a separate
skin folder for theme assets. All of your templates and assets are now stored in:
`app/design/frontend/<package>/<your_theme>` (in other words, the old location
for your templates).



You will soon see that unlike Magento 1.x where all the templates were stored in `app/
design/frontend/<package>/<theme>/template`, there are a number of folders, as
demonstrated in the screenshot below. 

![magento block layout structure](https://lh6.googleusercontent.com/XYQG9rNyAOSVF-9Li1ux9Lil7cixHq2DtNGfHr7tZCCFeDJRJtt0MH1uZRmawQsG9puj3wuz5xoFlLXxUycejDZjgK6MOwLBCKy-xkPPWgECsvmg6elBKchv9lZCDUiq1W_R1_DP)

Each one of these folders represents a module in **Magento 2** where templates or assets
are overridden in this theme. The location of the default versions of each module can be
found in `app/code/Magento`
Let’s take a look at the structure of a typical module.

![magento 2 code module structure](https://lh3.googleusercontent.com/mo90IzXUgudcUyEVT7MQRK7m7n1jKluWTDV_OuDQSaaIsuyXblw4b9roe9v5CSHOgJDjMpnDgz5GWiepTywHFQYWikJLwGiFuio0oIXWrp3qGRivLplmvFurtT-NvbEhg_cXMZnt)

Here is an example of the checkout module in a custom theme. As you can see, it
contains a folder for layout updates (more on that later) one for templates and a “web”
folder, which replaces the old `skin/frontend/<package>/<theme>` folder. However,
instead of having all your sitewide assets and JS in this folder, such items are now
organised per module - in this case, the Magento Checkout module.

Those of you with a keen eye may also have noticed that there is a template folder in
the web folder of this module. This is unique to a few Magento 2 modules (including
Checkout) where Magento 2 employs KnockoutJS for templating. We’ll look at
KnockoutJS in more detail in a later tutorial. These templates use .html files and internal
logic (i.e. no PHP is involved).

As explained earlier, if you want to override / amend the core modules’ templates and
JS, you will need to create an equivalent module folder in your theme that matches the
path(s) of the file(s) you wish to override / extend.

Taking another example, if you take a look in app/code/Magento you will see all of
the default modules used by Magento 2 core. If you want to override something in the
Catalog module, for example, you would then need to create a folder in your theme
called Magento_Catalog. This references the `<package_name>`, in this case the
“Magento” portion of app/code/Magento i.e. `app/code/<package>`, and then the
portion after the underscore refers to the module name. In this case, this is Catalog:
`app/code/<package>/<module>`

In other words, to override the contents of a module in `app/code/<package>/<
module>`  `app/code/<package>/<module>`, you will need to create a folder named
`<package>_<module>` in your theme.

Also note that you can only override the contents of the `view/frontend` portion of the
module within your theme (so `app/code/Magento/Catalog/view/frontend` maps to
`app/design/frontend/<your_package>/<your_theme>/Magento_Catalog` ). If you
need to override Controllers and Blocks, this is done in a different location and normally
by a backend developer, which is not covered in this guide.
