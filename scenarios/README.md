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
characters: ["miranda", "raphael"]
characterColors: {"miranda": "#3D6FA8", "raphael": "#9C6B2E"}
---
```

`characters` contient les identifiants des fiches de `personnages/` (nom du
fichier sans `.md`). Dans l'éditeur de scénario, cochez les personnages
concernés et choisissez leur couleur : toutes les occurrences de leur nom sont
colorées dans l'aperçu et à la lecture. Les couleurs doivent être au format
hexadécimal `#RRGGBB`. Les événements de la chronologie peuvent être associés à
un scénario depuis leur formulaire de modification ; le jalon affiche alors un
bouton pour ouvrir ce scénario.

Le corps prend en charge les titres `##`, listes `-`, tableaux, citations,
liens HTTP(S), **gras**, *italique*, `code` et
`***[éléments à arbitrer par le MJ]***` pour les placeholders rouges.
Les titres `##` à `####` alimentent le sommaire cliquable. Dans l'éditeur, le
menu « Insérer un modèle de scène » fournit des modèles Info MJ, description,
dialogue, roleplay, test, combat et note. Dans la lecture d'un scénario,
le bouton **Imprimer** ouvre la boîte d'impression du navigateur ; choisissez
une imprimante ou « Enregistrer au format PDF ».
Dans l'éditeur, la barre d'insertion se trouve sous la zone Markdown et le
bouton **Masquer l’aperçu** permet d'agrandir l'espace d'écriture.

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
