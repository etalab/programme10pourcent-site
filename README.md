# Programme 10% - Site web

Site de présentation du programme 10%

Le site est un fork du site [peren.gouv.fr](https://gitlab.com/peren/website/website) 

C'est un site statique utilisant le générateur de site statique [Hugo](https://gohugo.io/).


## Installation

* Installer hugo : voir les [instructions d'installation de Hugo](https://gohugo.io/getting-started/installing/).
* Installer node : voir les [instructions d'insatllation](https://lesbricodeurs.fr/articles/Comment-installer-npm-proprement/). 

Puis lancer les commandes suivantes: 

```
$ git clone git@github.com:etalab-ia/programme10pourcent.git
$ cd programme10pourcent/
$ cd themes/design-system-gouvfr && npm i && cd ../../
$ cp -r themes/design-system-gouvfr/node_modules/@gouvfr/dsfr/dist/ ./static/design-system-gouvfr
```

## Générer le site

```
$ git clone git@github.com:etalab-ia/programme10pourcent.git
$ cd programme10pourcent/
$ hugo serve
```

* Ouvrir dans un navigateur le lien : http://localhost:1313/

## Licence

Le contenu du site est publié sous [licence ouverte](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf) 
