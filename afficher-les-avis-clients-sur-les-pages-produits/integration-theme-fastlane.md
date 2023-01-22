---
description: >-
  Vous utilisez le thème Fastlane ? Suivez les étapes ci-dessous afin d'intégrer
  Trustreviews sur votre site web.
coverY: 0
---

# Thème Fastlane

## Afficher les avis clients sur ma page produit :

1. Rendez-vous dans votre menu Themes Shopify. (boutique en ligne -> modifier le code)
2. Cliquez sur le menu "Actions", puis sélectionnez "Modifier le code".
3. Ouvrez le menu ''SNIPPETS'' et en suite ''reviews.liquid''.
4. Copiez la ligne de code dans le cadre ci-dessous :

```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```

1. Collez la ligne de code ci-dessus où vous le souhaitez dans l'onglet ''reviews.liquid''.  Attention, collez la ligne de code **avant** le tag ''\</body>''. Effectuez un **cmd + f** (sur macbook) ou un **ctrl + f** (sur windows) et recherchez le tag ''\</body>''. En suite, collez la ligne de code où vous le souhaitez avant ce tag.

![Voici un exemple](../.gitbook/assets/IMG\_8152.JPG)

## Vérifiez le code ci-dessous :

1. Vérifiez dans la catégorie '' theme.liquid '' que le code ci-dessous est bien affiché. Copiez/collez ce code et rendez-vous dans\
   '' theme.liquid ''. Recherchez si ce code est affiché grâce aux commandes **cmd + f** (sur macbook) ou **ctrl + f** (sur windows).
2. &#x20;Si le code n'est pas affiché, collez-le avant le tag '' \</body> ''\
   Ce code est nécessaire pour que Trustreviews fonctionne correctement sur votre thème.&#x20;

```bash
{{ shop.metafields.trustreviews["global_html_body"] }}
```

![Voici un exemple](../.gitbook/assets/IMG\_8151.JPG)

{% hint style="warning" %}
Versions différentes - Thème Fastlane
{% endhint %}

Attention, il se peut qu'en fonction de la version de votre thème Fastlane, l'intégration se fait comme pour les [_**thèmes classiques**_](integration-manuelle.md). Si l'intégration ci-dessus ne fonctionne pas, veuillez suivre la méthode des [_**thèmes classiques**_](integration-manuelle.md).
