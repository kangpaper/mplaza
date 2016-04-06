---
layout: kb
title: How to create Magento 2 theme Step by step
permalink: /kb/how-to-create-magento-2-theme.html
published: true
categories: magento-2-tutorial magento-2-frontend
tags: magento-2 how-to block template layout theme
---


There are number of improvements to the way themes are managed and set up in
Magento 2. The use of the theme.xml definition file, introduced in Magento 1.9, and
a new fallback system, are two of the most significant improvements. The fallback
system in Magento 2 works in a similar way to Magento 1.x, but has the added
advantage that you can select unlimited parent themes to inherit from / fallback to
- all via the theme.xml file in your theme. 


Let’s say you want to create a brand new theme based on the new Magento “Blank”
theme. First, you would create a new folder in `app/design/frontend` called, for example
Session/default. You would then create a theme.xml file in this directory (it is probably
best to copy it from `app/design/frontend/Magento/blank/theme.xml`), name your
theme, and choose any parent. In this case, we want Magento 2’s Blank theme.

So your theme.xml file should look something like this:

```xml
<theme xmlns:xsi=”http://www.w3.org/2001/XMLSchema-instance”
xsi:noNamespaceSchemaLocation=”../../../../lib/internal/
Magento/Framework/Config/etc/theme.xsd”>
 <title>Session Default</title>
 <parent>Magento/blank</parent>
</theme>

```

### Theme structure

#### Folder structure

```xml
app/design/frontend/<Vendor>/
├── <theme>/
│   ├── etc/
│   │   ├── view.xml
│   ├── web/
│   │   ├── images
│   │   │   ├── logo.svg
│   ├── registration.php
│   ├── theme.xml
│   ├── composer.json
```

<Vendor> is theme vendor. e.g: mageplaza
<theme> is theme name. e.g: ultimate


Ok, let's go

## Creating a Magento theme folder

Creating a folder for the theme:

* Go to `app/design/frontend`
* Creating a vendor folder `app/design/frontend/<vendor>` e.g: `app/design/frontend/mageplaza`
* Create a theme folder `app/design/frontend/<vendor>/<theme>` e.g: `app/design/frontend/mageplaza/ultimate`
	```xml
			app/design/frontend/
		├── mageplaza/
		│   │   ├──...ultimate/
		│   │   │   ├── ...
		│   │   │   ├── ...

	```



## Declare your theme

Now we have folder `app/design/frontend/mageplaza/ultimate` , now create a file named `theme.xml` that define basic information about theme such as: Name, parent theme (in case your theme inherits from an existing theme), preview image

```xml
<theme xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:framework:Config/etc/theme.xsd">
     <title>Mageplaza Ultimate</title> <!-- your theme's name -->
     <parent>Magento/blank</parent> <!-- the parent theme, in case your theme inherits from an existing theme -->
     <media>
         <preview_image>media/preview.jpg</preview_image> <!-- the path to your theme's preview image -->
     </media>
 </theme>

```

## Composer package

**Composer** is a tool for dependency management in PHP. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you.

To distribute your theme as a package, add a `composer.json` file to the theme directory and register the package on a packaging server. 

`composer.json` example:

```xml
{
    "name": "mageplaza/ultimate",
    "description": "N/A",
    "require": {
        "php": "~5.5.0|~5.6.0|~7.0.0",
        "magento/theme-frontend-blank": "100.0.*",
        "magento/framework": "100.0.*"
    },
    "type": "magento2-theme",
    "version": "100.0.1",
    "license": [
        "OSL-3.0",
        "AFL-3.0"
    ],
    "autoload": {
        "files": [
            "registration.php"
        ]
    }
}
```


## registration.php file

You can add the following content to register the theme to Magento 2

```php
<?php
/**
 * Copyright © 2015 Magento. All rights reserved.
 * See COPYING.txt for license details.
 */
\Magento\Framework\Component\ComponentRegistrar::register(
    \Magento\Framework\Component\ComponentRegistrar::THEME,
    'frontend/mageplaza/ultimate',
    __DIR__
);
```

You should change mageplaza, ultimate to your vendor, theme name.


## Creating static files, folders

In a design, there are many static files such as javascript, css, images and fonts. They are stored in separate folders in `web` of theme package.

Here are the structure

```xml
app/design/<area>/mageplaza/ultimate/
├── web/
│ ├── css/
│ │ ├── source/ 
│ ├── fonts/
│ ├── images/
│ ├── js/

```

##### Tips

In Magento 2, theme or extension development, when you update any files in `app/design/<area>/mageplaza/ultimate/web` folder, you have to static folders which located at `pub/static` and `var/view_preprocessed` Otherwise, you still there is no change in frontend.


## Configure catalog product images

As you can see in the theme strucure I mentioned above, there is a file called `etc/view.xml`. This is configuration file. This file is required for Magento theme but it is optional if exists in parent theme.

Go to `app/design/<area>/mageplaza/ultimate/` and create a folder `etc` and file `view.xml`
You can copy the `view.xml` file in parent theme such as **Blank theme** `app/design/frontend/Magento/blank/etc/view.xml`

Ok, let update the image configuration for catalog product grid page.

```xml
...
    <image id="category_page_grid" type="small_image">
        <width>250</width>
        <height>250</height>
    </image>
...

```

In view.xml, image properties are configured in the scope of <images module="Magento_Catalog"> element:

```xml
<images module="Magento_Catalog">
...
<images/>
```


Image properties are configured for each image type defined by the `id` and `type` attributes of the `<image>` element:

```xml
<images module="Magento_Catalog">
	<image id="unique_image_id" type="image_type">
	<width>100</width> <!-- Image width in px --> 
        <height>100</height> <!-- Image height in px -->
	</image>
<images/>
```


