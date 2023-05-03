---
description: >-
  Manual integration with classic themes. If stars are not automatically
  displayed when downloading the Trustreviews app, please follow these steps:
coverY: 0
---

# Classic themes

{% hint style="danger" %}
```
Watch out for new updates to Shopify themes. It is possible that
your classic theme has become a 2.0 theme.
So follow the 2.0 theme steps if necessary.
```
{% endhint %}

1. ```
   Go to your Shopify Themes menu. (online store -> Themes)
   ```
2. ```
   Click on the "Actions" menu, then select "Edit Code".
   ```
3. ```
   Open the section you use for product pages (usually this is called
   product-template.liquid or product.liquid, but some themes work differently).
   ```
4. ```
   Copy the line of code below:
   ```
5. ```
   Paste it where you want the stars to appear on the product page
   (we recommend pasting the code under the product title), then save
   your file.
   ```

```
<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```

```
Here is an example on the Debut theme:
```

![](<../.gitbook/assets/Afficher les étoiles Trustreviews.PNG>)

![](<../.gitbook/assets/affichage d'étoiles trustreviews thèmes classiques.png>)

