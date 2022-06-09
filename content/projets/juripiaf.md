---
title: "Analyse de corpus de textes juridiques à partir de la brique PIAF"
summary: Le projet vise à développer un moteur de recherche sémantique appliqué au corpus de conditions générales d'utilisation en français des services en ligne collecté par [OpenTermsArchive](https://opentermsarchive.org/fr). Sur le modèle de [PIAF appliqué au corpus service-public.fr](https://github.com/etalab-ia/piaf_agent), cet outil devrait permettre d'explorer et de comparer plus facilement les mentions légales de différents services en ligne. 
responsible: Lucas Verney (PEReN)
date: 2022-05-18T13:00:00+01:00
images: 
- /img/image-nlp.png
---

##### Les objectifs 
Les objectifs seraient de :
* Déployer une instance de https://github.com/etalab-ia/piaf_agent sur le corpus de mentions légales afin de disposer d'un premier démonstrateur.
* Itérer sur cette base afin d'affiner le modèle de NLP sous-jacent au périmètre des textes juridiques, ceci afin de pouvoir avoir une vue transverse des déclinaisons d'une même clause entre les différents services (exemple : "comment exercer mon droit à la portabilité des données ?" présenterait les extraits pertinents des CGUs de tous les services collectés).
* Reproduire et étoffer https://explore.usableprivacy.org/ sur des mentions légales en langue française en développant notamment des annotations automatiques pour lier des mentions présentes dans les CGUs à des obligations législatives.

##### Exemples de cas d'usage
En s'appuyant sur le corpus des conditions générales d'utilisation en français, ce projet vise également à enrichir le projet PIAF avec des capacités adaptées de traitement du langage naturel sur des corpus juridiques, qui pourraient être réutilisées dans d'autres contextes (textes législatifs, etc.).

##### Domaines techniques 
* NLP 
* Search 

##### Les profils recherchés
* Data scientist 
* Développeur 

##### Ressources utiles 
* La consolidation du dataset est effectuée en continu par OpenTermsArchive : https://opentermsarchive.org/fr.
* Une bibliographie d'outils similaires sur lesquels pourraient s'appuyer ce projet a été réalisée, notamment https://usableprivacy.org/ (en anglais).

