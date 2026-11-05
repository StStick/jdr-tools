# jdr-tools

## Chronologie de campagne

Le site est publié sur GitHub Pages par l'action `.github/workflows/pages.yml`.
Pour activer la publication la première fois, ouvrir **Settings > Pages** sur
GitHub et sélectionner **GitHub Actions** comme source de déploiement.

À chaque push sur `main` qui modifie `main.html` ou `json_save/`, l'action :

- publie `main.html` comme page d'accueil ;
- choisit la sauvegarde `version_JJ-MM-AA.json` dont la date est la plus récente ;
- la publie sous `latest.json`, que la page recharge à chaque ouverture.

Pour publier une nouvelle chronologie, ajouter le fichier JSON daté dans
`json_save/` et pousser le changement sur `main`. La page recharge les données
publiées à chaque ouverture ; les modifications faites dans l'interface restent
locales au navigateur jusqu'à leur exportation et leur ajout à `json_save/`.

**Attention :** GitHub Pages est public. Les événements marqués « Secret MJ »
restent cachés dans l'interface en mode joueurs, mais leur contenu est lisible
dans `latest.json`.
