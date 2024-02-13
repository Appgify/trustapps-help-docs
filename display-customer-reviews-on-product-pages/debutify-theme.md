---
description: >-
  Manual integration with Debutify. If customer reviews are not automatically
  displayed on your product page by downloading the Trustreviews app, please
  follow these steps:
coverY: 0
---

# Debutify Theme

![](<../.gitbook/assets/Capture d’écran 2021-10-17 à 16.20.00.png>)

1. Go to your Shopify Themes menu. (online store -> Themes)
2. Click on the "Actions" menu, then select "Edit Code".

![](<../.gitbook/assets/Capture d’écran 2021-10-17 à 16.35.50.png>)

1. In the code search bar, search for ''review'' and 2 titles should appear below the ''SNIPPETS'' section (see screenshot below)
2. To display customer reviews on your product page, go to ''review-widget.liquid''.&#x20;
3. Copy and paste the line of code below:

```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```

Paste the line of code below the phrase: (\<div class="review-widget">) in the review-widget.liquid section.

![](<../.gitbook/assets/Afficher avis clients debutify.png>)

Last step - verification

1. Check in the ''theme.liquid'' category that the code below is displayed. Copy/paste this code and go to ''theme.liquid''. Check if this code is displayed using the commands cmd + f (on macbook) or ctrl + f (on windows).
2. &#x20;If the code is not displayed, paste it before the tag '' '' This code is required for Trustreviews to work properly on your theme.

```
{{ shop.metafields.trustreviews["global_html_body"] }}
```

![](<../.gitbook/assets/Capture d’écran 2021-10-17 à 15.55.25 (1).png>)
