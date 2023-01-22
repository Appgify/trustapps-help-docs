---
description: >-
  Si les avis ne s'affichent pas automatiquement en cliquant sur ''intégrer
  Trustreviews'' dans vos paramètres de l'application Trustreviews, veuillez
  suivre les étapes suivantes :
coverY: 0
---

# Thèmes 2.0 Dawn - Sense - Taste - etc

## Ajouter les avis clients sur mes pages produits. Themes 2.0 :

* Rendez-vous dans **boutique en ligne** -> **personnaliser**.
* Choisissez la page produit concernée.
*   Suivez les étapes sur la capture d'écran ci-dessous :&#x20;

    Rendez-vous en bas et cliquez sur ''**Ajouter une séction**'' et choisissez l'application ''Trustreviews'' (Voir 2ème photo). Déplacez le bloc d'avis clients Trustreviews où vous le souhaitez. **(Reviews Widget)**

![](<../.gitbook/assets/Capture d’écran 2022-06-30 à 16.44.17.png>)

![Lorsque vous cliquez sur ''ajouter un bloc'', sélectionnez l'application Trustreviews qui se trouve en bas. Choisissez le widget des avis. (Reviews widget)](<../.gitbook/assets/Capture d’écran 2022-06-30 à 16.01.08.png>)

## 2ème méthode :&#x20;

Vous pouvez également ajouter les avis grâce à la méthode manuelle. Cela consiste à ajouter le code manuellement. (Voir ci-dessous)

1. &#x20;Rendez-vous dans **boutique en ligne** -> **personnaliser**.
2. Choisissez la page produit par défaut.
3.  Suivez les étapes sur la capture d'écran ci-dessous :&#x20;

    \-> **Ajoutez une section** et choisissez ''**Liquid personnalisé**''
4. Glisser le ''Liquid personnalisé'' où vous voulez que les avis s'affichent. Dans cet exemple, nous allons placer les avis en dessous de la description produit. Donc nous avons déplacé le Liquid personnalisé vers le haut, en dessous de la description.
5. Copiez le code ci-dessous et collez-le dans votre Liquid personnalisé.
6. Sauvegardez vos changements.

```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```

![](<../.gitbook/assets/Capture d’écran 2021-11-10 à 19.59.49.png>)
