---
description: >-
  La couleur des étoiles en dessous de votre titre n'est pas la même que la
  couleur des avis clients ? Il est possible que cela arrive dans certains cas.
  Suivez les étapes ci-dessous :
coverY: 0
---

# Synchroniser la couleur des étoiles

![](<../.gitbook/assets/Capture d’écran 2021-11-10 à 20.35.39.png>)

1. Rendez-vous dans boutique en ligne -> Actions -> Modifier le code.
2. Cliquez sur **theme.liquid** et recherchez le **\</head>**.
3. Copiez le code ci-dessous et collez-le au dessus du **\</head>**. (Voir capture d'écran ci-dessous)

```
{{ shop.metafields.trustreviews["global_html_head"] }}
```

![Ceci est un exemple sur le thème Debut.](<../.gitbook/assets/Capture d’écran 2021-11-10 à 20.25.54.png>)

4\. Sauvegardez. En suite, rendez-vous sur votre site web et rafraîchissez la page. Rafraîchissez la page plusieurs fois si nécessaire, cela peut prendre quelques dizaines de secondes pour voir le changement.
