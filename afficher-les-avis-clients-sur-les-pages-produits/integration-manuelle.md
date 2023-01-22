---
description: >-
  Manual integration with classic themes. If customer reviews are not displayed
  automatically when downloading the Trustreviews app, please follow these steps
  ->
coverY: 0
---

# Classic themes

{% hint style="danger" %}
```
Watch out for new updates to Shopify themes. It is possible
that your classic theme has become a 2.0 theme. So follow
the 2.0 theme steps if necessary.
```
{% endhint %}

<pre><code><a data-footnote-ref href="#user-content-fn-1">Show customer reviews on my product page: #</a>
</code></pre>

1. To manually embed the Trustreviews tab on your product pages and display customer reviews at the bottom of your product page, follow these steps:
2. ```
   Go to your Shopify Themes menu. (online store -> edit code)
   ```
3. Click on the "Actions" menu, then select "Edit Code".
4. Open the section you use for product pages (usually called product.liquid / product-template.liquid / product-page.liquid / product-main.liquid, but some themes work differently).
5.  Copy the line of code in the box below:


6. Paste the entire line of code where you want customer reviews to appear. In order to display customer reviews at the very bottom of your page, please paste the code at the very bottom of the code page. Here is an example on the Debut theme:

{% code title="Line of code:" %}
```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```
{% endcode %}

_**`Here is an example on the Debut theme: #`**_

![](<../.gitbook/assets/Afficher les avis clients.PNG>)

```
The Trustreviews tab appears like this: #
```

![](<../.gitbook/assets/trustreviews onglet.png>)

[^1]: 
