---
layout: kb
title: How to Create Module in Magento 2 - Helloworld development series - Completed Guide
permalink: /kb/how-create-hello-world-module-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to development helloworld
---


We will discuss the topic of how to create Hello World module in Magento 2 in order to help you have the clearest and easiest way to create now. Remember that the concept of local/ community/ core/ folders only existed in Magento 1 and you will don’t use them for Magento 2. 

## To create Hello World module in Magento 2:

### Step 1: Create the folder of Hello World module

Name of the module is defined as “VendorName_ModuleName”. First part is name of the vendor and last part is name of the module:
For example: Magento_Helloworld, Mageplaza_Helloworld. Focus on following guide to create the folders:

~~~ php
  app/code/Mageplaza/Hello
~~~ 

### Step2: Add module.xml

Then, it is necessary to add the module.xml file

~~~ php
  app/code/Mageplaza/Hello/etc/module.xml
~~~

Contents would be:
~~~ xml
  <?xml version="1.0"?>
  <config xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:framework:Module/etc/module.xsd">
  <module name="Mageplaza_Hello" setup_version="0.0.1"/>
  </config>
~~~

### Step3: Add registration.php 

In this step, we will add registration.php as following guide:

~~~ php
  app/code/Mageplaza/Hello/registration.php
~~~

Contents would be: 

~~~ php
  <?php
  \Magento\Framework\Component\ComponentRegistrar::register(
      \Magento\Framework\Component\ComponentRegistrar::MODULE,
      'Mageplaza_Hello',
      __DIR__
  );
~~~

### Step 4: Enable the module

Finish the step 3, we have already created the `Hello World` module. And we will enable this module in this step

After create the module if you run the command as: 

~~~ php
  php bin/magento module:status
~~~

You should see the module is disable now: 

  List of disabled modules: 
  ``Mageplaza_Hello``
 
Follow exact guide to enable the module right now, let run the command as: 

~~~ php
  php bin/magento module:enable Mageplaza_Hello
~~~

Or other way, you can access the file: 

~~~ php
  app/etc/config.php
~~~

You will see a long list of modules there, just add your module as well

~~~ php
  ...
  'Mageplaza_Hello' => 1, 
  ....
~~~

Your module should be available now.

After this step, when you open your website in browser you will get an error saying 

  Please upgrade your database: Run "bin/magento setup:upgrade" from the Magento root directory.

Let run the command:

~~~ php
  bin/magento setup:upgrade
~~~

to fix the error. 
You can also see your module at System Configuration -> Advanced -> Disable Modules Output

### Step5: Create a Routes for the module

In this step, you should add an url known as a route so that you can display `Hello World`

Route’s in magento are divided into 3 parts: Route_id, controller and action as following example: 

``http://magentostore.com/index.php/route_id/controller/action``


To add route, it is necessary to add routes.xml file

~~~ xml
  Mageplaza/Hello/etc/frontend/routes.xml
~~~

since this is a frontend route, we added it in frontend/ folder else we need to add it to adminhtml/ folder

Content would be: 

~~~ xml
  <?xml version="1.0"?>
  <config xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="../../../../../../lib/internal/Magento/Framework/App/etc/routes.xsd">
    <router id="standard">
        <route id="mageplaza" frontName="mageplaza">
            <module name="Mageplaza_Hello" />
        </route>
    </router>
  </config>  
~~~

You should define ID and FrontName is the same because some mistakes maybe occur during your setup processing.

After define the first part of the route, the URL will be displayed as: 
  
  ``www.magentostore.com/mageplaza/*``

Then, you will continue define our controller, action

Your URL now should be as: 

  ``www.magentostore.com/mageplaza/hello/world``

The folder you need to create is: 

  ``Mageplaza/Hello/Controller/Hello/World.php``

That folder should contain the following content:

~~~ php
  <?php
  namespace Mageplaza\Hello\Controller\Hello;
 
  class World extends \Magento\Framework\App\Action\Action
  {
    public function __construct(
        \Magento\Framework\App\Action\Context $context)
    {
        return parent::__construct($context);
    }
     
    public function execute()
    {
        echo 'Hello World';
        exit;
    } 
  }

~~~

After finish all steps, the output “Hello World” should be displayed in your browser when you open the URL.
We hope our guide is very useful and effective for you.
