---
description: >-
  Intégration manuelle avec les thèmes classiques. Si les avis clients ne
  s'affichent pas automatiquement en téléchargeant l'app Trustreviews, veuillez
  suivre les étapes suivantes ->
coverY: 0
---

# Thèmes classiques

{% hint style="danger" %}
Attention aux nouvelles mises à jour des thèmes Shopify. Il est possible que votre thème classique soit devenu un thème 2.0. \
Suivez donc les étapes des thèmes 2.0 si nécessaire.
{% endhint %}

## Afficher les avis clients sur ma page produit :

1. Pour intégrer manuellement l’onglet Trustreviews à vos pages produits et afficher les avis clients en bas de votre page produit, procédez comme suit :
2. Allez dans votre menu Themes Shopify. (boutique en ligne -> modifier le code)&#x20;
3. Cliquez sur le menu "Actions", puis sélectionnez "Modifier le code".
4. Ouvrez la section que vous utilisez pour les pages de produits (généralement appelé product.liquid / product-template.liquid / product-page.liquid / product-main.liquid, mais certains thèmes fonctionnent différemment).
5.  Copiez la ligne de code dans le cadre ci-dessous :


6. Collez la ligne de code entière à l'endroit où vous voulez que les avis clients apparaissent. Afin d’afficher les avis clients tout en bas de votre page, veuillez coller le code tout en bas de la page du code. Voici un exemple sur le thème Debut :

{% code title="Ligne de code :" %}
```
<div id="trustreviews" class="page-width" data-product-id="{{product.id}}"> {{ product.metafields.trustreviews.iframe }}
</div>
```
{% endcode %}

## Voici un exemple sur le thème Debut :

![](<../.gitbook/assets/Afficher les avis clients.PNG>)

## L'onglet Trustreviews s'affiche comme ceci :

![](<../.gitbook/assets/trustreviews onglet.png>)
