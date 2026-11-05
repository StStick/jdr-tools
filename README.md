# jdr-tools

## Chronologie de campagne

Le site est publié sur GitHub Pages par l'action `.github/workflows/pages.yml`.
Pour activer la publication la première fois, ouvrir **Settings > Pages** sur
GitHub et sélectionner **GitHub Actions** comme source de déploiement.

À chaque push sur `main` qui modifie `main.html`, `json_save/`, `scenarios/`
ou `personnages/`, l'action :

- publie `main.html` comme page d'accueil ;
- choisit la sauvegarde `version_JJ-MM-AA.json` dont la date est la plus récente ;
- la publie sous `latest.json`, que la page recharge à chaque ouverture ;
- publie les scénarios Markdown de `scenarios/` dans le catalogue du site ;
- génère le catalogue des fiches depuis les fichiers `.md` de `personnages/`.

Pour publier une nouvelle chronologie, ajouter le fichier JSON daté dans
`json_save/` et pousser le changement sur `main`. La page recharge les données
publiées à chaque ouverture ; les modifications faites dans l'interface restent
locales au navigateur jusqu'à leur exportation et leur ajout à `json_save/`.

Les scénarios se rédigent dans l'onglet **Scénarios**. Les brouillons et les
modifications restent dans le stockage local du navigateur ; pour les partager,
télécharger le fichier `.md` et l'ajouter au dossier `scenarios/`, puis pousser
le changement sur `main`. Le format et les encadrés disponibles sont décrits
dans [`scenarios/README.md`](./scenarios/README.md).

L'onglet **Personnages** affiche les fiches PJ/PNJ et permet de les rechercher
ou de filtrer par type. Chaque fiche est un fichier indépendant dans
[`personnages/`](./personnages/) : ajoutez un `.md` pour créer une fiche ou
supprimez le fichier correspondant pour retirer un personnage. Le format est
documenté dans [`personnages/README.md`](./personnages/README.md).

**Attention :** GitHub Pages est public. Les événements marqués « Secret MJ »
restent cachés dans l'interface en mode joueurs, mais leur contenu est lisible
dans `latest.json`, les scénarios et les fiches personnages sont accessibles
dans les fichiers Markdown publiés. Le site avertit les visiteurs, mais les
données publiées restent accessibles publiquement.
