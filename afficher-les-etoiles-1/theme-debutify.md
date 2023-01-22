---
description: >-
  Intégration manuelle avec Debutify. Si les étoiles ne s'affichent pas
  automatiquement en téléchargeant l'app Trustreviews, veuillez suivre ces
  étapes :
coverY: 0
---

# Thème Debutify

![Suivez-les étapes ci-dessous pour afficher les étoiles en dessous du titre de votre produit sur le thème DEBUTIFY.](<../.gitbook/assets/Capture d’écran 2021-10-17 à 15.48.04.png>)

1. Allez dans votre menu Themes Shopify. (boutique en ligne -> Themes)
2. Cliquez sur le menu "Actions", puis sélectionnez "Modifier le code".

![](<../.gitbook/assets/Capture d’écran 2021-10-17 à 16.35.50.png>)

1. Dans la barre de recherches des codes, recherchez ''review'' et 2 titres devraient apparaître en dessous de la section ''SNIPPETS'' (Voir capture d'écran ci-dessous)
2. Pour afficher les étoiles en dessous du titre de votre produit, rendez-vous dans ''**review-badge.liquid**''.&#x20;
3. Copiez et collez la ligne de code ci-dessous :

```
<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```

Collez la ligne de code en dessous de la phrase : **(% if badge\_template == "product" %)** dans la section **review-badge.liquid.**

![](<../.gitbook/assets/Afficher etoiles debutify.png>)

## Dernière étape - vérification

1. Vérifiez dans la catégorie '' theme.liquid '' que le code ci-dessous est bien affiché. Copiez/collez ce code et rendez-vous dans\
   '' theme.liquid ''. Recherchez si ce code est affiché grâce aux commandes **cmd + f** (sur macbook) ou **ctrl + f** (sur windows).
2. &#x20;Si le code n'est pas affiché, collez-le avant le tag '' \</body> ''\
   _Ce code est nécessaire pour que Trustreviews fonctionne correctement sur votre thème._

```
{{ shop.metafields.trustreviews["global_html_body"] }}
```

![](<../.gitbook/assets/Capture d’écran 2021-10-17 à 15.55.25.png>)
