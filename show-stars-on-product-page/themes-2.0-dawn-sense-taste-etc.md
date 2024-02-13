---
description: >-
  If stars are not automatically displayed by clicking on 'integrate
  Trustreviews' in your Trustreviews app settings, please follow these steps:
coverY: 0
---

# Themes 2.0 Dawn - Sense - Taste - etc

```
Add stars to my product pages. Themes 2.0: #
```

* ```
  Go to online store -> customize.
  ```
* ```
  Choose the relevant product page.
  ```
* ```
  Follow the steps on the screenshot below:

  In your product information, click on ''Add a block'' and choose the
  ''Trustreviews'' application (See 2nd photo). Move the Trustreviews block
  below your product title
  ```

![](<../.gitbook/assets/Capture d’écran 2022-06-30 à 15.59.21.png>)

![Lorsque vous cliquez sur ''ajouter un bloc'', sélectionnez l'application Trustreviews qui se trouve en bas. Choisissez le widget des étoiles. (Star Ratings)](<../.gitbook/assets/Capture d’écran 2022-06-30 à 16.01.08.png>)

<pre><code>2nd method: <a data-footnote-ref href="#user-content-fn-1">#</a>
</code></pre>



```
You can also add the stars using the manual method. This consists of
adding the code manually. (See below)
```

1. ```
   Go to online store -> customize.
   ```
2. ```
   Choose the default product page.
   ```
3.  Follow the steps on the screenshot below:

    ```
    In your product information, click on ''Add block'' and choose
    ''Custom liquid''. Move the custom Liquid below your product title.
    ```
4. ```
   Copy the code below and paste it into the custom Liquid. The stars will appear.
   ```

```
<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```

![ ](<../.gitbook/assets/Capture d’écran 2021-11-10 à 20.04.42.png>)

```
Stars home page:
```

If you want to display the stars on a product on your home page, the same method applies but the code is different. Copy/paste and use the code below:

```
{% raw %}
{%- assign product = section.settings.product -%}
{% endraw %}

<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```

[^1]: 
