---
description: >-
  Manual integration with Debutify. If stars are not automatically displayed
  when downloading the Trustreviews app, please follow these steps:
coverY: 0
---

# Debutify Theme

![Suivez-les étapes ci-dessous pour afficher les étoiles en dessous du titre de votre produit sur le thème DEBUTIFY.](<../.gitbook/assets/Capture d’écran 2021-10-17 à 15.48.04.png>)

1. ```
   Go to your Shopify Themes menu. (online store -> Themes)
   ```
2. Click on the "Actions" menu, then select "Edit Code".

![](<../.gitbook/assets/Capture d’écran 2021-10-17 à 16.35.50.png>)

1. ```
   In the code search bar, search for ''review'' and 2 titles should appear
   below the ''SNIPPETS'' section (See screenshot below)
   ```
2. ```
   To view the stars below your product title, go to
   ''review-badge.liquid''.
   ```
3. ```
   Copy and paste the line of code below:
   ```

```
<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```

```
Paste the line of code below the phrase: (% if badge_template == "product" %)
in the review-badge.liquid section.
```

![](<../.gitbook/assets/Afficher etoiles debutify.png>)

```
Last step - verification
```

1.  ```
    Check in the ''theme.liquid'' category that the code below is displayed.
    Copy/paste this code and go to
    ```

    \


    ```
    ''theme.liquid''. Find if this code is displayed using the commands
    cmd + f (on macbook) or ctrl + f (on windows).
    ```
2. ```
   If the code is not displayed, paste it before the tag '' </body> ''
   This code is required for Trustreviews to work properly on your theme.
   ```

```
{{ shop.metafields.trustreviews["global_html_body"] }}
```

![](<../.gitbook/assets/Capture d’écran 2021-10-17 à 15.55.25.png>)
