# Personnages de Yeast Eaters

Chaque personnage a sa propre fiche Markdown dans ce dossier. Le catalogue du
site et les fichiers publiés sont générés automatiquement à partir de ces
fiches lors du déploiement GitHub Pages.

Pour ajouter un personnage, créez un fichier `.md` avec un nom stable et les
métadonnées suivantes :

```markdown
---
name: "Nom du personnage"
kind: PJ
---

## Identité
Informations d'identité.

## Histoire
Éléments d'histoire.
```

`kind` doit être `PJ` ou `PNJ`. Chaque titre `##` devient une rubrique de la
fiche affichée sur le site ; son contenu peut utiliser le Markdown (gras,
italique, listes, citations).

Pour retirer un personnage du site, supprimez simplement son fichier `.md` de ce
dossier. Poussez les changements sur `main` pour publier les ajouts ou retraits.

**Attention :** GitHub Pages est public. Ne mettez pas ici d'informations qui
ne doivent pas être visibles par les visiteurs du site.
