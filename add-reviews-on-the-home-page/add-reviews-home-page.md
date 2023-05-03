---
coverY: 0
---

# Add reviews - home page

```
Show customer reviews on my homepage:
```

1. ```
   Go to your Shopify Themes menu. (online store -> edit code)
   ```
2. ```
   Click on the "Actions" menu, then select "Edit Code".
   ```
3. ```
   Open the section you use for the homepage, it's called: index.liquid
   ```
4. ```
   Copy the line of code in the box below:
   ```

```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```

6\. Paste the line of code below "content-for-index". As in the screenshot below:

![](<../.gitbook/assets/Capture d’écran 2021-11-01 à 20.30.57.png>)
