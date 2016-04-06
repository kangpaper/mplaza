---
layout: kb
title: How To Create Magento 2 Theme Ultimate Guide
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

![how to create magento 2 theme](https://lh4.googleusercontent.com/rC25rdFRLLZYkV4JI376EbWhoIzw2n7s1furHA-BqhS1VNYX8QY64cUuHldhNqA2fHbQ4bALASeo4xqwG5obUvYCvL5hXGQ7lQyIqvLiRWG3WVPBwlB66a2IZiISEgd7jvb9dYSn)

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

```
app/design/frontend/mageplaza/
├── ultimate/
│   ├── etc/
│   │   ├── view.xml
│   ├── web/
│   │   ├── images
│   │   │   ├── logo.svg
│   ├── registration.php
│   ├── theme.xml
│   ├── composer.json
```

`<Vendor>` is theme vendor. e.g: mageplaza

`<theme>` is theme name. e.g: ultimate


Ok, let's go

## Creating a Magento theme folder

Creating a folder for the theme:

* Go to `app/design/frontend`
* Creating a vendor folder `app/design/frontend/<vendor>` e.g: `app/design/frontend/mageplaza`
* Create a theme folder `app/design/frontend/<vendor>/<theme>` e.g: `app/design/frontend/mageplaza/ultimate`

```
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

#### Tips

In Magento 2, theme or extension development, when you update any files in `app/design/<area>/mageplaza/ultimate/web` folder, you have to static folders which located at `pub/static` and `var/view_preprocessed` Otherwise, you still there is no change in frontend.


## Configure catalog product images

As you can see in the theme strucure I mentioned above, there is a file called `etc/view.xml`. This is configuration file. This file is required for Magento theme but it is optional if exists in parent theme.

Go to `app/design/<area>/mageplaza/ultimate/` and create a folder `etc` and file `view.xml`
You can copy the `view.xml` file in parent theme such as **Blank theme** `app/design/frontend/Magento/blank/etc/view.xml`

Ok, let update the image configuration for catalog product grid page.

```xml
<image id="category_page_grid" type="small_image">
    <width>250</width>
    <height>250</height>
</image>

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



## Declare Theme Logo

In Magento 2 default, it uses `<theme_dir>/web/images/logo.svg`, in your theme, you can change to different file format such as png, jpg but you have to declare it.


Logo size should be sized `300x300px`  and you open file `<theme_dir>/Magento_Theme/layout/default.xml`

```xml
<page xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:framework:View/Layout/etc/page_configuration.xsd">
    <body>
        <referenceBlock name="logo">
            <arguments>
                <argument name="logo_file" xsi:type="string">images/custom_logo.png</argument>
                <argument name="logo_img_width" xsi:type="number">300</argument> 
                <argument name="logo_img_height" xsi:type="number">300</argument>
            </arguments>
        </referenceBlock>
    </body>
</page>
```


## Basic layout elements


The basic components of Magento page design are blocks and containers.

A container exists for the sole purpose of assigning content structure to a page. A container has no additional content except the content of included elements. Examples of containers include the header, left column, main column, and footer.


![magento 2 layout](https://lh5.googleusercontent.com/1qGHXaoKgz7pb_anKa21HABo_bo3w2YX-Hn87cAMDJrHJAbQyZVQLKsKmsDEqzCS2xon441mGg_ZMmqT_O8rKt0pAEwyT6wgd8CxKboqxwQd4SLR1IVqmdRsBtiHffNcAp3TlZKl)



## Layout files types and conventions

#### Module and theme layout files

The following terms are used to distinguish layouts provided by different application components:

* Base layouts: Layout files provided by modules. Conventional location:
	* Page configuration and generic layout files: `<module_dir>/view/frontend/layout`
	* Page layout files: `<module_dir>/view/frontend/page_layout`
* Theme layouts: Layout files provided by themes. Conventional location:
	* Page configuration and generic layout files: `<theme_dir>/<Namespace>_<Module>/layout`
	* Page layout files: `<theme_dir>/<Namespace>_<Module>/page_layout`


### Create a theme extending file

Rather than copy extensive page layout or page configuration code and then modify what you want to change, in the Magento system, you only need to create an extending layout file that contains the changes you want.

To add an extending page configuration or generic layout file:

```xml
<theme_dir>
 |__/<Namespace>_<Module>
   |__/layout
     |--<layout1>.xml
     |--<layout2>.xml

```

For example, to customize the layout defined in `<Magento_Catalog_module_dir>/view/frontend/layout/catalog_product_view.xml`, you need to add a layout files with the same name in your custom theme, like following:

`<theme_dir>/Magento_Catalog/layout/catalog_product_view.xml`

```xml
<theme_dir>
 |__/<Namespace>_<Module>
   |__/page_layout
     |--<layout1>.xml
     |--<layout2>.xml
```


### Override base layouts

Overriding is not necessary if a block has a method that cancels the effect of the originally invoked method. In this case, you can customize the layout by adding a layout file where the canceling method is invoked.

To add an overriding base layout file (to override a base layout provided by the module):
Put a layout file with the same name in the following location:

```xml
<theme_dir>
  |__/<Namespace_Module>
    |__/layout
      |__/override
         |__/base
           |--<layout1>.xml
           |--<layout2>.xml
```


These files override the following layouts:

- `<module_dir>/view/frontend/layout/<layout1>.xml`
- `<module_dir>/view/frontend/layout/<layout2>.xml`


### Override theme layouts

To add an overriding theme file (to override a parent theme layout):

```xml
<theme_dir>
  |__/<Namespace_Module>
    |__/layout
      |__/override
         |__/theme
            |__/<Parent_Vendor>
               |__/<parent_theme>
                  |--<layout1>.xml
                  |--<layout2>.xml

```

These files override the following layouts:


- `<parent_theme_dir>/<Namespace>_<Module>/layout/<layout1>.xml`
- `<parent_theme_dir>/<Namespace>_<Module>/layout/<layout1>.xml`


#### Tips!
	- Changing block name or alias. The name of a block should not be changed, and neither should the alias of a block remaining in the same parent element.
	- Changing handle inheritance. For example, you should not change the page type parent handle.


Congrats! Now you have your first simple Magento 2 theme. You can try to create a complexible theme later.


Ref: Devdocs.magento.com, Stackoverflow.com
