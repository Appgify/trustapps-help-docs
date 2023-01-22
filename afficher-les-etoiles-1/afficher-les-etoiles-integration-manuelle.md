---
description: >-
  Intégration manuelle avec les thèmes classiques. Si les étoiles ne s'affichent
  pas automatiquement en téléchargeant l'app Trustreviews, veuillez suivre ces
  étapes :
coverY: 0
---

# Thèmes classiques

{% hint style="danger" %}
Attention aux nouvelles mises à jour des thèmes Shopify. Il est possible que votre thème classique soit devenu un thème 2.0. \
Suivez donc les étapes des thèmes 2.0 si nécessaire.
{% endhint %}

1. Allez dans votre menu Themes Shopify. (boutique en ligne -> Themes)
2. Cliquez sur le menu "Actions", puis sélectionnez "Modifier le code".
3. Ouvrez la section que vous utilisez pour les pages de produits (généralement, cela s'appelle product-template.liquid ou product.liquid, mais certains thèmes fonctionnent différemment).
4. Copiez la ligne de code ci-dessous : \

5. Collez-le à l'endroit où vous souhaitez que les étoiles apparaissent sur la page produit (nous vous recommandons de coller le code sous le titre du produit), puis enregistrez votre fichier.&#x20;

```
<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```

## Voici un exemple sur le thème Debut :

![](<../.gitbook/assets/Afficher les étoiles Trustreviews.PNG>)

![](<../.gitbook/assets/affichage d'étoiles trustreviews thèmes classiques.png>)

