---
description: >-
  If stars are not automatically displayed by clicking on 'integrate
  Trustreviews' in your Trustreviews app settings, please follow these steps:
cover: ../.gitbook/assets/Untitled (1).jpg
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Add stars widget to theme

### Add stars to my product pages. (For themes 2.0)

* Go to online store -> customize
* Choose the relevant product page.
* Follow the steps on the screenshot below:

  In your product information, click on ''Add a block'' and choose the
  ''Trustreviews'' application (See 2nd photo). Move the Trustreviews block
  below your product title

![](<../.gitbook/assets/Capture d’écran 2022-06-30 à 15.59.21.png>)

### Show stars on home page

If you want to display the stars on a product on your home page, the same method applies but the code is different. Copy/paste and use the code below:

```
{% raw %}
{%- assign product = section.settings.product -%}
{% endraw %}

<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```
