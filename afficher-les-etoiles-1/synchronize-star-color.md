---
description: >-
  The color of the stars below your title is not the same as the color of the
  customer reviews? This may happen in some cases. Follow the steps below:
coverY: 0
---

# Synchronize star color

![](<../.gitbook/assets/Capture d’écran 2021-11-10 à 20.35.39.png>)

1. Go to Online Store -> Actions -> Edit Code.
2. Click on theme.liquid and search for the .
3. Copy the code below and paste it above the . (See screenshot below)

```
{{ shop.metafields.trustreviews["global_html_head"] }}
```

![This is an example on the Debut theme.](<../.gitbook/assets/Capture d’écran 2021-11-10 à 20.25.54.png>)

4\. Save. Next, go to your website and refresh the page. Refresh the page several times if necessary, it may take a few tens of seconds to see the change.
