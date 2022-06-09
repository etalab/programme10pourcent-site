---
title: "SIRETisation"
date: 2022-05-18T13:00:00+01:00
responsible: Alexis Eidelman (DARES) + Etalab
summary: La recherche du numéro SIRET d’immatriculation d’un établissement dans le répertoire administratif SIRENE de l'INSEE à partir de son libellé et lieu géographique à l’aide des API actuelles ne donne pas toujours un résultat satisfaisant. Plusieurs administrations travaillent à améliorer cette recherche, le but de ce projet serait de répertorier les outils existants et de contribuer à de nouveaux développements.
images: 
- /img/image-siret.png
---

##### Les objectifs

Pour répondre à la problématique de cette « sirétisation », l’idée serait d’enrichir la base SIRENE  à l’aide d'informations contextuelles (libellé d'usage, informations géographiques, etc.), produites généralement en interne par plusieurs administrations via des annotations ou des tableaux structurés contenant des listes d’entreprises et de métadonnées1 qui pourrait être mobilisées à cette fin d’amélioration du codage. 

Par exemple, pour un nom de marque franchisé qui n’existe pas tel quel dans le référentiel SIRENE, ce serait le bon numéro Siret de son gérant qui lui serait attribué (ce qui n'est pas toujours le cas). On peut citer également l’exemple des changements de noms (rachat par une unité légale, cession, fusion, transfert, etc.) mais qui n’est pas appliqué instantanément dans les sources de données.

Au final, il s’agirait de créer une version enrichie de SIRENE avec des alias d’usage, s’éloignant de la dénomination sociale proprement dite et de permettre aux administrations qui emploient parfois ces noms d'usage de retrouver les entreprises qu'elles recherchent.

Un autre aspect de la « sirétisation » est son historique : les établissements peuvent évoluer assez rapidement dans le temps (rachat par une unité légale, cession, fusion, transfert, etc.), cette dimension peut alors faire évoluer les réponses, car elle entraine parfois un changement du numéro Siret.

Il s’agit ensuite de permettre de requêter dans la base, en utilisant au mieux tous les éléments à notre disposition pour pouvoir nuancer le matching sur le nom : la recherche d’un établissement sur lequel on a quelques informations - mêmes imprécises - est en effet d’autant plus aisée que cette base de données de référence contient des informations sectorielles, géographiques, administratives, etc. qui aident à trancher des identifications ambiguës. Ces informations permettent non seulement d’éliminer des candidats inexacts issus d’une recherche flou « fuzzy matching », mais aussi d’imaginer des mots-clefs synonymes si la recherche par information-clef n’est pas concluante.

##### Exemples de cas d'usage

Cette problématique de SIRETisation est partagée par un très grand nombre d'administrations. Parmi les très nombreux cas d'usage on peut citer notamment :
- La statistique publique (INSEE, DREES, DARES, etc.)
- La SIRETisation des établissements de santé connus par leurs numéros FINES
- L'évaluation de politiques publiques


##### Domaines techniques

- Développement d'API
- Recherche d'information dans un index (par exemple via le moteur Elasticsearch)

##### Les profils recherchés

- Compétences ponctuelles en ingénierie de données pour déterminer la structure que pourraient prendre ces tableaux de données.
- Expertise pour déterminer les meilleures métriques
- Compétences métiers pour déterminer des alias
- Gestion de projet

##### Ressources utiles

- L'API SIRENE de l'INSEE : [catalogue des API de l'INSEE](https://api.insee.fr/catalogue/)
- La solution SocialGouv du Ministère du Travail : [lien github](https://github.com/SocialGouv/recherche-entreprises) et [interface de SocialGouv](https://recherche-entreprises.fabrique.social.gouv.fr/)
- Le catalogue des entreprises (bientôt plus maintenu ?): (https://entreprise.api.gouv.fr/catalogue/)
- L'API "Annuaire Entreprises" développée à Etalab qui repose sur une base de données nourrie avec SIREN et un moteur Elastic search : [Annuaire Entreprise](https://annuaire-entreprises.data.gouv.fr/)
- Le projet Insee AMI IA "Améliorer l’identification de l’établissement employeur dans le recensement de la population" : [description du projet](https://www.etalab.gouv.fr/intelligence-artificielle-decouvrez-les-15-nouveaux-projets-selectionnes/)
- Potentiellement l'API Entreprises, qui s'adresse aux entreprises qui veulent obtenir des informations les concernant : [API entreprise](https://entreprise.api.gouv.fr/catalogue/)