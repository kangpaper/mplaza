---
layout: kb
title: How to create Configurable Product in Magento 2
permalink: /kb/how-create-configurable-product-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to configure create product
---

You can create a Configurable Product in Magento 2 through many variations and the Configurable Product differs from a Single product by a drop-down list of option for each variation. That means it is simple for you to track inventory for the product variation because an option is actually a simple product with a unique SKU. This advance is the thing you could have if creating a simple product with custom options, however,  it is impossible to track inventory for each variation by that way. Although it take much time to set up a configurable product, you can save time in the long term of your business’s growing. Therefore, the configurable product type is a good choice for products with multiple options.

![configurable product](https://lh5.googleusercontent.com/Q7lBZjyL_ffLG99huWc4tTjfdHJ-VhWAndFGlpFdDCJxxMheRVxa1Y7NdBclV2TsYZcv5r1G2qNF4ESB5b2uD0sA72aezra4jkn7LYG2i3UDV1F3l32x14d0nq9DRFSJ7BwE7qE1)

## Process overview:

      Part 1: Create the Configurable Product
        Step 1: Select the Product Type is Configurable Product
        Step 2: Select the Product Template 
        Step 3: Complete the Required Fields
        Step 4: Complete the Remaining Product Details
        Step 5: Save and Continue
        
      Part 2: Add Configurations
        Step 1: Select the Attributes
        Step 2: Enter the Attribute Values
        Step 3: Configure the Images, Price and Quantity
        Step 4: Generate the Product Configurations
        Step 5: Publish the Products
        Step 6: Configure the Shopping Cart Thumbnails (Optional)
        Step 7: Final, check your result by view the Products in your store

# Part 1: Create the Configurable Product

## Step 1: `Select the Product Type is Configurable Product`

* On the Admin sidebar, click `Products`. Then under `Inventory`, select `Catalog`
* In the upper-right corner on the `Add Product` menu, select `Configurable Product`

![add configurable product](https://lh3.googleusercontent.com/pU19_sp-qxOJfogNuyQsi0w8wNhOHWeqFyVwVypo0pGmTrUR1Aiv1CxL4_sFVJ6UBHz6_TvZ9TgnUL3huCLUoZHGQYfuPcij8cBI-DbQ34MjdZ8fPLRztmzBN6pRr1ug5vkF_V8Q)

## Step 2: `Select the Product Template`

To choose Product Template, you can follow one of two ways: 
* Enter directly the name of the template that you want to choose in the `Search` box
* Click in the list and choose the template that you want to use.
Remember that, a Configurable Product require the option of available fields must include at least one drop-down attribute. 

![choose template](https://lh4.googleusercontent.com/HR--rUQ1_6ZdZLHkp1KsI4W__1p7tuHF9jVQPKPFAAVh4WJU3U_CxWfbc9EwERQx1zFSmOyls5hb93AeFekvyC62SPZQ5JHI87Vl1JXIXoFGFu_6YUkRU7wHMdqQsuJpNlZghHkM)

## Step 3: `Complete the Required Fields`

* In the `Product Details` section, enter the product `Name`.
* Either accept the default `SKU` that is based on the product name, or enter another value.
* Enter the product `Price`.
* If necessary, change the `Tax Class`. The default setting is “Taxable Goods.”
* Because the product is not yet ready to publish in your catalog, set the `Product Online` switch to the “Off” position.

## Step 4: `Complete the Remaining Product Details`

* (Optional) You can add an image that represents the configurable product as a whole, or wait until later when you set up the configurations. In this example, we use an image that shows the top in all three colors. An image uploaded here becomes the image of the “parent product.”
  * Drag an image from your desktop, and drop it on the camera tile in the `Images and Videos` box.
  * In the box, click the `camera tile`, and navigate to the image file on your computer. Then, select the image, and click `Open`.
A placeholder appears until an image is uploaded. If you prefer, you can later add video to the gallery.
* The `Quantity` field is not available because it’s determined by each product variation.
* To assign the product to a `Category`, do one of the following:
  * Start typing to find a match. Then, choose the`Category`.
  * Click the `Show List` icon to view the `Category` tree. Then, drill down through the available categories, and tap each category that you want to assign to the product.
  * Click `New Category`. Enter the `Category Name` and choose the `Parent Category` to determine its position in the menu structure. Then, click `Create Category`.
* Enter the product `Description` directly into the text box, and format as needed. Then, click `Submit`. You can also use the `WYSIWYG Editor`for additional control.

![product detail](https://lh4.googleusercontent.com/cqe3xvmQ2_Iu_gLwspeR8KhEjO5xMkFC4dqsQdAk429g5HtO_3vjhfEKv8-7s2klqg0sukUZ_1zbJ1l6joPY60BSnduz2wu_rN1hyOhUkdorHrznz0SoG-EhTWUJfj0Z6B57v1Qc)

## Step 5: `Save and Continue`

This is a good time to save your work. In the next step, you’ll set up the configurations for each variation of the product.
* In the upper-right corner, click `Save`.
* Continue with `Adding Configurations`. 

# Part 2: Add Configurations

Follow 7 steps to know how to configure multiple colors and multiple sizes for each Configurable Product. It is simple when you only need to create Simple Products with unique SKUs and then combine all of variations together. Remember to keep an eye on the progress bar at the top of the page, which will show where you are in the process and what the next step for you is.

![progress-bar](https://lh6.googleusercontent.com/07VI_SMmd4d1DJfnkkYbCcIFbXbXXHUJ7VpB6BvDZts-X9g10hmZbrbdLFLW--ePb4BF8a6dkK40Ui4gfwczVB60g8A4VIz3Od3MwOXTTnYTMcD24LnpWNZ5mrVdROGL5dpjHuMp)

## Step 1: `Select the Attributes`

* At the bottom of `Product Details`, expand the `Configurations` section. Then, tap `Create Configurations`.

![configuration](https://lh5.googleusercontent.com/cho7MGheraRYCV-ZW7DWhBHwBkpActw-hekxLkQljUZleYl16lpAgC3UJI-kvTWxAoUpZc0PfXaE1TOVbxSzZlkhknSPJwVzq7Q97I9HxaDiF-gxZ2hkEG6uUsZGH7sJJ5YbNws9)

* Mark the checkbox of each attribute that you want to set.
* If you need to add a new attribute, go to tap `Create New Attribute`,and `Save Attribute` after completing the attributes properties. Then, mark the checkbox to select the attribute.
* In the upper-right corner, tap `Next`.

![set-attributes](https://lh3.googleusercontent.com/RR1ug8eHwl-j7gdyN67MlMdFtI8I-a98I6rABPTSCMW00mnVtmyUqdzo0Pc35FZ4jgHQrWafbSvzdj_JPJBeqfbBA7i6Qf8SgN-Lj6ggFjvOPD6btD1NeK47vx9hAnSw1gLpFsTF)

## Step 2: `Enter the Attribute Values`

* Mark the checkbox of each variation of the product.
* Add a new value by clicking `Create New Value`. Enter the value of the new input, then tap the Enter arrow.
* Do the same to each attribute you have chosen before.

  The order of attributes can be rearranged by dragging-dropping to a new position.

* In the upper-right corner, tap `Next`.

![choose-color](https://lh3.googleusercontent.com/XQ_9SB1izxrPvB9M3iWZt1mcK69H70OVSwetdmoiSNcl2-3wqGS4_OlcTeLQwB9qtHiC8ieoIWdBa_0xtGJAgCA1jhi3SMwcI4hn8wik2P8B8jSIR_FRBT2UPCwyDITv6CNI001O)

## Step 3: `Configure the Images, Price and Quantity`

The images, pricing and quantity will be set in this step while you can choose only one option for each of them. It is possible to select the same or unique setting or you can skip the setting for now.

* Choose the configuration options that apply.

### `Configure the Images`

#### Method 1: `Apply a Single Set of Images to All SKUs`

   * Select `Apply single set of images to all SKUs`.
   * Choose the desire image from your browse.

![use-same-image-for-all-SKUs](https://lh6.googleusercontent.com/FNS-abPQs4DhZuwNfUIP_HEaCorkU1SDnlNO7a5_fVl_n4X9BjiBVsadFI3bMcPhB0Rw4muYH8cN1oQdIbLgT9hfRIGepm8IRNim1iAPHznOIzqr5NI3RlnG8fiGm6xsfPOaOH7U)

#### Method 2: `Apply Unique Images for Each SKU`

   * Select `Apply unique images by attribute to each SKU`.
   * Select the attribute, for example: color. If your shopper choose a specific color, the image will appear.
   * Allow uploading differents image for each attribute, either browse to the images or drag them to the box. If want to delete the image, tap the bin icon.
  
![unique-image-per-SKU](https://lh3.googleusercontent.com/HWX0L8WmpVBhQV9zsV78nozP8vrW8_XO-WNWc0e27qkXybahNrq2qcvmiWCwXJd01VBBAL80DO8uOm44WkN32qJx_RW1ec37BBPT5D6FPDuFZr2F7eaDTo16Kp0ss_VliYEdHe3N)
  
### `Configure the Prices`

#### Method 1: `Apply the Same Price to All SKUs`

   * Select `Apply single price to all SKUs`.
   * Enter the `Price`.

![same-price-for-all-SKUs](https://lh6.googleusercontent.com/Yv16qRcKgQyoreAUQYiybhjMXad10I-edHPIuVAEQ9L_gv3glhWWSEDoBBrQDwL4MojFCCAZ9CEADRAeKIvOQb6OGD5AfhqpP62NZtQgbUeWgzbOrpPqgMxQ8Nxln3aAT06KGO1l)

#### Method 2: `Apply a Unique Price for Each SKU`

   * Select `Apply unique prices by attribute to each SKU`.
   * Select the attribute you want to offer a specific price.
   * Enter the `Price`.
 
![unique-price-per-SKU](https://lh6.googleusercontent.com/29ZmZpPwYTFaOsDJb-RsaXPd4If4Kg9ZFfcsup0gmZTdQAJHrl-nb4qQrTQXp2rR10ZFFYb2F6PbQfH9PCVNFLj8p0vDSmNiE_S4tA_nlkao-DPskb8p2UWsY8l4OyZrSWGraG6w)

### `Configure the Quantity`

#### Method 1: `Apply the Same Quantity to All SKUs`

   *  Select `Apply single quantity to each SKU`.
   *  Enter the `Quantity`.
 
![same-quantity-for-al-SKUs](https://lh3.googleusercontent.com/PYfgKSgaQfx2JyG8c4nAeczOszi2fFDxyjLfKdBtTW_0sNyjHkhcTyBd9xagZ2_pcM0W-glslvkvuJ0Y37L7WpLyplb3S0kQwf-vNSsAwLXcbsFKywD7rzX0U3qAdO5LjYUJgWWK)

#### Method 2: `Apply a Unique Quantity by Attribute`

   *  Select `Apply unique quantity by attribute to each SKU`.
   *  Enter the `Quantity`

![unique-quantity-per-SKU](https://lh5.googleusercontent.com/1wKIY16XUoMEDjv_3B5DOSrkEcbEhrSYsRvXeXh5rb3AZZLc3Y7y2nl7x44rYoy8NaiJAVYXyz9EJRkd7y_ZATNmq47bKpQGjZy1nKdYrZtaVGtVuQoz3U5yDhHIbHQOC3WabI_G)

* Tap `Next` in the upper-right corner to continue.

##  Step 4: `Generate the Product Configurations`

* Check your list of products. When you are ready, tap `Generate Product` to add the product to your catalog. The product variations now appear at the bottom of Product Details in the Configuration section.
* If want to edit, tap `Edit Configuration`.

![generate-products](https://lh3.googleusercontent.com/KvShYrcfNKiLk3oQnOxmDjKHqivJ0jL5ohBYRZ9QqcAtI3gYX8wVqnqOMCtlgT4FehKS8cpjhRn4qJVW_MpvG27ak4ay6eQIaGUI4-HDAXdNpaFniVG3q9DeEXFVA6NrYvl1d-36)

## Step 5: `Publish the Products`

* Switch `Product Online` to the **On** or **Off** depending on whether you are ready or not to publish the products in the catalog. 
* On the `Save` menu, choose `Save & Close`to finish the generating.

![save-close](https://lh4.googleusercontent.com/fZ5guX9L4UZE-6UbJcnLXUMxIMw-A6lzZn1ltJs-AkhuW_l4oCBoheEpmtx7oFfvcDClJ0UfZIDmy2RDjSHBxuXXke3ZKl6daQatrsZKKmIPr0G4P8ZAgFLmkOndublddUPN5Xin)

* Remember to click on `Cache Management` link in the system message to fush new cache and refresh the invalid cache.
* On the Admin sidebar, tap Products. Your new configurable product and its variations appears in the grid at the top of the list.

## Step 6: `Configure the Shopping Cart Thumbnails` (Optional)

Approve to set a different image for each variation in the shopping cart thumbnail if you need.

* On the Admin sidebar, tap `Stores`. Then under Settings, choose `Configuration`.
* In the Sales tab, choose `Checkout`. Then, expand the `Shopping Cart` section.
* In the `Configurable Product Image`, select “Product Thumbnail Itself”.
* Tap `Save Config` to complete.

![shopping-cart-configurable-product](https://lh5.googleusercontent.com/U7xTOF7oOaSFiLoqMDeLSb_U8QQ_91qhXMolA8TbsWyw3segcLRf9yYLwc8_HBgpC3jN-Zhu4KuPZnAzZRspPUGl9Dc122IFSobuTZ_aLSyn6dgE_XThSd1F2zx2bPcdJ7e57ijW)

## Step 7: `Final, check your result by view the Products in your store`

As soon as the product is online, tap the arrow in the `Admin` in the upper-right corner, and choose `Customer View` to see them on the frontend.

![customer-view](https://lh6.googleusercontent.com/UfYyq-GxxQmdZJFWZy4uBj6YgWQqzBpStt7ReFAAL_VfZxfa6Jc_PIeFPAyPeXeB_ayluCWg4zNqzPow8jfMscDDTr_87ag68olsJW2M-sXmULS0pgJGfIcACGpR7xoxat0r9MYf)

# Important Notes

* A configurable product is a simple product with many options chosen from drop-down list.

* A value of a drop-down list is based on an attribute of the “Dropdown” input type. The drop-down attributes must be included in the attribute set, which is then used as a template for the configurable product. 

* Store Admin can set other thumbnail image in the shopping cart from the configurable product record, or from the product variation. 


