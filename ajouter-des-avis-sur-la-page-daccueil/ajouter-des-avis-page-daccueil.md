---
coverY: 0
---

# Ajouter des avis - page d'accueil

## Afficher les avis clients sur ma page d'accueil :

1. Allez dans votre menu Themes Shopify. (boutique en ligne -> modifier le code)
2. Cliquez sur le menu "Actions", puis sélectionnez "Modifier le code".
3. Ouvrez la section que vous utilisez pour la page d'accueil, cela s'appelle: **index.liquid**&#x20;
4. Copiez la ligne de code dans le cadre ci-dessous :

```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```

6\. Collez la ligne de code en dessous de ''**content-for-index**". Comme sur la capture d'écran ci-dessous:

![](<../.gitbook/assets/Capture d’écran 2021-11-01 à 20.30.57.png>)
