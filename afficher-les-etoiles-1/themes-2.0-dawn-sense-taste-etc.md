---
description: >-
  Si les étoiles ne s'affichent pas automatiquement en cliquant sur ''intégrer
  Trustreviews'' dans vos paramètres de l'application Trustreviews, veuillez
  suivre les étapes suivantes :
coverY: 0
---

# Thèmes 2.0 Dawn - Sense - Taste - etc

## Ajouter les étoiles sur mes pages produits. Themes 2.0 :

* Rendez-vous dans **boutique en ligne** -> **personnaliser**.
* Choisissez la page produit concernée.
*   Suivez les étapes sur la capture d'écran ci-dessous :&#x20;

    Dans les informations de votre produit, cliquez sur ''**Ajouter un bloc**'' et choisissez l'application ''Trustreviews'' (Voir 2ème photo). Déplacez le bloc Trustreviews en dessous du titre de votre produit

![](<../.gitbook/assets/Capture d’écran 2022-06-30 à 15.59.21.png>)

![Lorsque vous cliquez sur ''ajouter un bloc'', sélectionnez l'application Trustreviews qui se trouve en bas. Choisissez le widget des étoiles. (Star Ratings)](<../.gitbook/assets/Capture d’écran 2022-06-30 à 16.01.08.png>)

## 2ème méthode :&#x20;

Vous pouvez également ajouter les étoiles grâce à la méthode manuelle. Cela consiste à ajouter le code manuellement. (Voir ci-dessous)

1. Rendez-vous dans **boutique en ligne** -> **personnaliser**.
2. Choisissez la page produit par défaut.
3.  Suivez les étapes sur la capture d'écran ci-dessous :&#x20;

    Dans les informations de votre produit, cliquez sur ''**Ajouter un bloc**'' et choisissez ''**Liquid personnalisé**''. Déplacez le Liquid personnalisé en dessous du titre de votre produit.
4. Copiez le code ci-dessous et collez-le dans le Liquid personnalisé. Les étoiles vont apparaître.

```
<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```

![ ](<../.gitbook/assets/Capture d’écran 2021-11-10 à 20.04.42.png>)

## Étoiles page d'accueil :

Si vous souhaitez afficher les étoiles sur un produit de votre page **d'accueil**, la même méthode est d'application mais le code est différent. Copiez/collez et utilisez le code ci-dessous :&#x20;

```
{% raw %}
{%- assign product = section.settings.product -%}
{% endraw %}

<a href="#trustreviewsFrame"><div class="trustreviews-rating" data-id="{{ product.id }}" data-rating="{{ product.metafields.trustreviews.avg_rating }}" data-raters="{{ product.metafields.trustreviews.num_reviews }}"></div></a>
```
