# Scénarios Yeast Eaters (Markdown)

Les fichiers de scénario publiés doivent être placés dans ce dossier, au format
`.md`, avec un nom de fichier stable et sans espaces (par exemple
`scenario-01-doliprane.md`). Le workflow les ajoute automatiquement au catalogue
du site après un push sur `main`.

Chaque fichier commence par ces métadonnées :

```markdown
---
title: "Titre du scénario"
date: "15 février 2313"
secret: false
---
```

Le corps prend en charge les titres `##`, listes `-`, tableaux, citations,
liens HTTP(S), **gras**, *italique*, `code` et
`***[éléments à arbitrer par le MJ]***` pour les placeholders rouges.

## Encadrés de la charte

Ouvrir un encadré par sa balise et le fermer par une ligne `:::` :

```markdown
::: desc
Texte d'ambiance à lire aux joueurs.
:::

::: mj
Secret d'intrigue réservé au MJ.
:::

::: dial Miranda
**Miranda :** « *Vous avez trois minutes avant le traçage.* »
:::

::: rp Négociation
Décrivez l'objectif de la scène et les possibilités d'improvisation.
:::

::: event Test de Perception
DD 15 : les PJ repèrent la caméra dissimulée.
:::

::: combat
Précisez l'initiative, les renforts et les conditions de fuite ou reddition.
:::

::: prep
Informations et matériel à préparer avant la séance.
:::

::: note
Indices critiques et conséquences à archiver pour la campagne.
:::
```

Les styles d'encadrés suivent la charte graphique du projet. Les brouillons créés
dans le site restent dans le navigateur ; télécharger le `.md` puis le déposer
dans ce dossier pour le publier. GitHub Pages étant public, ne publiez pas ici
de secret qui ne doit pas être accessible aux joueurs.
