---
description: >-
  Are you using the Fastlane theme? Follow the steps below to embed Trustreviews
  on your website.
coverY: 0
---

# classic themes

Show customer reviews on my product page:

1. Go to your Shopify Themes menu. (online store -> edit code)
2. Click on the "Actions" menu, then select "Edit Code".
3. Open the ''SNIPPETS'' menu and then ''reviews.liquid''.
4. Copy the line of code in the box below:

```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```

1. Paste the above line of code wherever you want in the ''reviews.liquid'' tab. Be careful, paste the line of code before the '''' tag. Do a cmd + f (on macbook) or a ctrl + f (on windows) and search for the tag ''''. Then, paste the line of code where you want before this tag.

![Voici un exemple](../.gitbook/assets/IMG\_8152.JPG)

Check the code below:

1. Check in the ''theme.liquid'' category that the code below is displayed. Copy/paste this code and go to ''theme.liquid''. Check if this code is displayed using the commands cmd + f (on macbook) or ctrl + f (on windows).
2. &#x20;If the code is not displayed, paste it before the tag '' '' This code is required for Trustreviews to work properly on your theme.

```bash
{{ shop.metafields.trustreviews["global_html_body"] }}
```

![Voici un exemple](<../.gitbook/assets/IMG\_8151 (1).JPG>)

{% hint style="warning" %}
Different Versions - Fastlane Theme
{% endhint %}

Please note, depending on the version of your Fastlane theme, the integration may be done as for the classic themes. If the above integration does not work, please follow the classic themes method.
