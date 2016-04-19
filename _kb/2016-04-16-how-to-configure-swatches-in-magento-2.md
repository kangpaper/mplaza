---
layout: kb
title: How to configure Swatches in Magento 2
permalink: /kb/how-to-configure-swatches-in-magento-2.html
published: true
categories: magento-2 magento-2-tutorial
tags: magento-2 how-to configure swatches
---
In the shopping online, customers have high expectations to the attributes of product including color, pattern, or texture. Differ from configurable products, color can be indicated by a visual swatch, text swatch, or a dropdown input control, swatches can be used on the product page, in product listings, and in layered navigation. 

![swatches-on-product-page](https://lh5.googleusercontent.com/puFTfFf7Z1wpCaEcAqPYjoVp3-l054_wyDODaCVVHeafShRTfc7ykbceNfI6AzIPQezar-RYkWDgSPc4IR7eVQTaNQDQAMepFbVoC8yShROiEsbxj6Ig8nSgfQzszq1f4DGE2Hap)

## Text-Based Swatches

If you did not set a specific image for color swatch, a text-based will appear instead of true color and behave in the same way as a swatch with an image.

![text-based-swatches](https://lh3.googleusercontent.com/rTNTHwB13L5y60kuQG_bY4tEOec36gotfI8aclwIaAHax3LcLFEk3xp0j9gjIvETCAFjphCx_sTwFBjDHYFWomhoU2mgti3nuy65NoN4tO6i0rX5lLRnNX_jH7rsIyjBVGBT0kEg)

When text-based swatches are used to show the available sizes, any size that is not available is crossed out.

![text-based-swatches](https://lh4.googleusercontent.com/VQbYmprmm7RnmDKukioErGkgABk8FbMeCBjGEqHvez19p9IhkuTPuq4iQTl-nlo9aRkpj9vpwjxMSZw4N5L0r8KLcJrrGFaOrglmYHgUfU3EfKmWxbzBuuDElHyPwBgaJPPdPQ0_)

## Swatches in Layered Navigation 

The swatches including color swatches and text-based swatches can be also used in the layered navigation. 

![swatches-in-layered-navigation](https://lh4.googleusercontent.com/TOYg5igV8wTj9cDVQTgOdEyuQBD8llDLPZuYgt4iMopYQeHPFcCF5556CgL25iTTyFVpYZhTbKMsPVpA0llKeqpURjrjq3LGzL4HsxszYB52VW5XUZbZF6rmYTlzyUU6Vb_DveKP)

## Creating Swatches

### Step 1: Create the Swatches

Apply one of the following method to create the swatches.

#### Method 1: Add a Color Swatch
* Identify the exact color for your product.
* On the Admin sidebar, `Stores > Attributes > Product`.
* In the grid, find and edit the `Color` attribute.
* Set `Catalog Input Type for Store Owner` to **Visual Swatch**.
* Under `Manage Swatch`, tap `Add Swatch` to add a new definition to the bottom of the list. Then, do the following:

![manage-swatch-values'](https://lh6.googleusercontent.com/BTxy-nMWRz_cxlrwWFPbjMIZgAvaJle4J2mmg1Z9fE55BFVhkyncDxInAoRfWu_3TfkBcgv9CO521qJu7UhG7qHSKmBg-XWKokJzOh6cpsK47YwJQeQVkJn2qeK1jx6Y2EOErE2p)

  * On the swatch menu, select `Choose a color`.
  
  ![choose-swatch-color](https://lh6.googleusercontent.com/AijfZt0XOhNt7nB9boV8f5MFX5-6xdtlTBIMjT4z1pNlM8-UB7krPXlAHT2Rtk54K7oRB-9YJQ2oudE6ITanAMjNChjtd__Os_0i_BDzxh-d1Oap90r-nisNQLiop150_bNVzr3z)
  
  * In the color picker, enter the six numbers that represent the hexadecimal value of the new color in the `#` field, and press the Backspace key to delete the current value. Then tap the `Color Wheel` button in the lower-right corner to save the swatch.
  
  ![hexadecimal-color](https://lh6.googleusercontent.com/sSIX52EXSNuNRHUnFFzQREPx8xryvvvMhddYuxfcDNkCd1fBkdSiA5uJ7kCwM-3TxFQukYuv9heGpx4eLNnrU7l5QpoRyV2a-lMThxD3rr20EPgsPe_oOPa7wnlX43a-UfHtksXX)
  
  * Enter the label for the color in the Admin and Default Store View.
  * Mark the checkbox under the `Is Default` to set the default color as you need.
  * Enable to change the order when tap the icon in the top left of **Manage Swatch** table and drag it to the new position.
* When complete, tap `Save Attribute`, then flush the cache in `Cache Management` tab.
* Finally, go to `Edit` mode in each product, and update `Color` attribute with the correct swatch. To update multiple products at the same time, follow the steps below.

#### Method 2: Upload a Swatch Image
* Collect the swatch image that is correct for your product.
* On the Admin sidebar, `Stores > Attributes > Product`.
* In the grid, find and edit the `Color` attribute.
* Set `Catalog Input Type for Store Owner` to **Visual Swatch**.
* Under `Manage Swatch`, tap `Add Swatch` to add a new definition to the bottom of the list. Then, do the following:
  * On the swatch menu, select `Upload a file`.
  
  ![upload-swatch-file](https://lh3.googleusercontent.com/6fo-dNjEI_KyPD_JrLzq2IucOFkeJOl3JgbkYFfpIO60hLNq1QzfUUkDnUVVMMMn65dwmWPkSEdUKmYj9PicUYWSBBzJ6YTbBkggPLAF9UlgjxoCfv8dmXZHFcs2k2yJ37OApWUN)
  
  * Choose the desired image from your computer.
  * Repeat these steps for other swatch images.
  * Enter the label for the color in the Admin and Default Store View.
* When complete, tap `Save Attribute`, then remember to flush the cache in `Cache Management` tab.
* Finally, go to `Edit` mode in each product, and update `Color` attribute with the correct swatch. To update multiple products at the same time, follow the steps below.

### Step 2: Update your product
* On the Admin sidebar, Products > Inventory > Catalog.
* `Filter` the list by Name or SKU to include only the applicable products.

![filter-attributes](https://lh5.googleusercontent.com/P_ICzw_mmRyLpg5BSQ6Rd1B0dVlt-QvqgfQ8-t8-IE3J7AvsZQm7yw8ZOWbCVZJSPo00z0PNI5g0E_fIpPla6TUXMwpJa6LkFswS8F5GiiTaPrCn2VZT3QIj-WYrdaNQ2rQLhZoh)

* Mark the checkbox of each product that you want the swatch to apply. And then, set the `Actions` control to **Update Attributes**.

![update-attributes](https://lh5.googleusercontent.com/rUxmshKjkyXRNZ6fkUzVlEhM-im1nW5BqwtiRHP8QN0U51FdzgL1jknsQZFFbrOlpWC9WI3BBq7kzgayDJeZskwhXn-4rvBjmAejN0bBD0uvkVxf6B7syaqJ-31ru5g8tWU4fQvu)

* Look down to the `Color` attribute, and mark the Change checkbox.

![change-color](https://lh6.googleusercontent.com/FipdYDxAsPTQd_CfMj7zzZqHhzwGLgY9ETwi1pMiTU8MNYTwjZSrYLZ0068ieIsb0x9ptJswi23JLbuLfOdNf6ZzP0j4T4dl5uHcr1h_AYWHgs-enF0IXL6Rkc_4QKWeactWDea2)

* Tap `Save` to apply the swatch. Then remember to flush the cache in the `Cache Management` tab.

![color-frontend](https://lh3.googleusercontent.com/9AoX7qfP9lCkot1X1ZFo4kWU2HX-jmnDlUc5Ic1IjphJFEwxQm9DSxsTQmbFVj9bgEHP7sy-8yQvU7X1N1-nafEVoUzlxixLM09U5OdrZ-Cn_9WMhW-ifEQIwnT-S_zzdTxbxLsI)
