---
description: >-
  If reviews are not automatically displayed by clicking 'integrate
  Trustreviews' in your Trustreviews app settings, please follow these steps:
coverY: 0
---

# Themes 2.0 Dawn - Sense - Taste - etc

## Add customer reviews to my product pages. Themes 2.0:

* Go to online store -> customize.
* Choose the relevant product page.
*   Follow the steps on the screenshot below:

    Go to the bottom and click on ''Add a section'' and choose the ''Trustreviews'' application (See 2nd photo). Move the Trustreviews customer reviews block wherever you want. (Reviews Widget)

![](<../.gitbook/assets/Capture d’écran 2022-06-30 à 16.44.17.png>)

![When you click on ''add block'', select the Trustreviews app which is at the bottom. Choose the reviews widget. (Reviews widget)](<../.gitbook/assets/Capture d’écran 2022-06-30 à 16.01.08.png>)

## 2nd method:&#x20;

You can also add reviews using the manual method. This consists of adding the code manually. (See below)

1. &#x20;Go to online store -> customize.
2. Choose the default product page.
3. Follow the steps on the screenshot below: -> Add a section and choose ''Custom Liquid''
4. Drag the ''Custom Liquid'' where you want the notices to appear. In this example, we'll place reviews below the product description. So we moved the custom Liquid to the top, below the description.
5. Copy the code below and paste it into your custom Liquid.
6. Save your changes.

```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```

![](<../.gitbook/assets/Capture d’écran 2021-11-10 à 19.59.49.png>)
