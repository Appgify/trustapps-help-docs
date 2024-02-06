---
description: 'How to add section in theme code manually? Follow the steps below:'
coverY: 0
---

# Add section code:

1. Go to theme code editor.
2. Create a new liquid file in 'sections' folder.
3. Copy the following code:
    
```
<div id="trustreviews" class="page-width" data-product-id="{{ product.id }}">
    {{ product.metafields.trustreviews.iframe }}
</div>

{{ shop.metafields.trustreviews["global_html_body"] }}

{% schema %}
{
  "name": "TrustReviews Widget",
  "presets": [{
		"name": "All reviews - Grid",
		"category": "Trustreviews"
	}]
}
{% endschema %}
```