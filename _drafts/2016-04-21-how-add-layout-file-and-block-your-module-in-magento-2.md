---
layout: kb
title: How to add layout file and block to your module in Magento 2
permalink: /kb/how-add-layout-file-and-block-your-module-in-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to create downloadable product
---

In the previous recipe, we supported the easiest way to create the Mageplaza_Hello module. And this topic, we will continue by discussing how to add layout file and block to your module. 
With adding layout file, we can arrange the specific structure of the page.

## To add layout file and block to your module in Magento 2

### Step 1:

In this step we will use “Hello World” module that created in previous recipe and display this module by using magento’s layout system.
The contents would be: 

~~~ php
  <?php
  namespace Excellence\Hello\Controller\Hello;
 
 
  class World extends \Magento\Framework\App\Action\Action
  {
    protected $resultPageFactory;
    public function __construct(
        \Magento\Framework\App\Action\Context $context,
        \Magento\Framework\View\Result\PageFactory $resultPageFactory)
    {
        $this->resultPageFactory = $resultPageFactory;       
        return parent::__construct($context);
    }
     
    public function execute()
    {
        return $this->resultPageFactory->create(); 
    } 
  }
~~~

### Step 2: Setup the Layout file

Move to configure the layout file. The module that include all layout file in Magento 2 is `"view/frontend/layout"` folder. We need to create sepetarly layout file for every URL (route). The folder should be defined as: 

~~~ php
  Excellence/Hello/view/frontend/layout/excellence_hello_world.xml
~~~

The content in the file would be: 

~~~ php
  <?xml version="1.0"?>
  <page xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" layout="1column" xsi:noNamespaceSchemaLocation="../../../../../../../lib/internal/Magento/Framework/View/Layout/etc/page_configuration.xsd">        
    <referenceContainer name="content">
        <block
            template="content.phtml"
            class="Excellence\Hello\Block\Main"
            name="excellence_test"/>
    </referenceContainer>
  </page>
~~~

### Step 3: Setup the Blocks file

Our block file would be displayed at the folder: 

~~~ php
  Excellence\Hello\Block\Main
~~~

The block file would be included the following contents:

~~~ php
  <?php
  namespace Excellence\Hello\Block;
  
  class Main extends \Magento\Framework\View\Element\Template
  {   
     public function __construct(
         \Magento\Framework\View\Element\Template\Context $context
     )
      {
         parent::__construct($context);
      }
      protected function _prepareLayout()
     {
         
     }
 }
~~~

### Step 4: Setup the Template file

Templates for a module will be displayed at `“view/frontend/templates”` folder. The file would be necessarily created now is: 

~~~ php
  Excellence/Hello/view/frontend/templates/content.phtml
~~~

Next, add content: 

~~~ php
  <h1><?php echo __('Hello World'); ?></h1>
~~~

