# Personnages de Yeast Eaters

Chaque personnage a sa propre fiche Markdown dans ce dossier. Le catalogue du
site et les fichiers publiés sont générés automatiquement à partir de ces
fiches lors du déploiement GitHub Pages.

Pour ajouter un personnage, créez un fichier `.md` avec un nom de fichier stable
et ces métadonnées :

```markdown
---
name: "Nom du personnage"
kind: PNJ
category: "New Right"
---

## Personnalité
Personnalité, comportement et façon de s'exprimer.

## Histoire
Origines, événements marquants et situation actuelle.

## Objectif
Ce que le personnage cherche à accomplir ou ce qui le motive.
```

`name` est le nom affiché, `kind` doit être `PJ` ou `PNJ`, et `category` permet
de classer le personnage par faction ou groupe. Les catégories existantes sont
proposées par le formulaire de création et servent de filtre dans le site.
Chaque fiche doit contenir exactement les trois rubriques `Personnalité`,
`Histoire` et `Objectif`, dans cet ordre. Leur contenu peut utiliser le
Markdown (gras, italique, listes, citations).

Dans l'onglet **Personnages**, le bouton **Créer un personnage** télécharge un
fichier Markdown à partir de ce modèle. GitHub Pages ne peut pas écrire dans le
dépôt : ajoutez le fichier téléchargé dans ce dossier puis poussez le changement
sur `main` pour le publier.

Pour retirer un personnage du site, supprimez simplement son fichier `.md` de ce
dossier. Poussez les changements sur `main` pour publier les ajouts ou retraits.

**Attention :** GitHub Pages est public. Ne mettez pas ici d'informations qui
ne doivent pas être visibles par les visiteurs du site.
