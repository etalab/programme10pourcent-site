---
title: "Faciliter l’association de sources de données géographiques issues de divers producteurs (INSEE, IGN, collectivités locales…)"
date: 2022-05-18T13:00:00+01:00
summary: Rassembler les données géographiques de l'IGN et les référentiels administratifs de l'INSEE dans un point d'entrée clair et normalisé (catalogue et API) pour faciliter l’harmonisation et l’association de données géographiques

responsible: Lino Galiana (INSEE)
images: 
- /img/image-ign-insee.png
---
 
#### La problématique identifiée:
 
De plus en plus de producteurs de données proposent des sources géolocalisées qui nécessitent des enrichissements avec des données de contexte (populations locales, niveau de vie de l’environnement…)  ou des contours géographiques (limites administratives, bâtiments ou lieux publics à proximité…). Par exemple, lorsqu’on désire représenter des données par une carte, la création de fonds de carte implique d’aller chercher un shapefile produit par l’IGN et d’associer les polygones au code officiel géographique (COG) de l’année en question. La représentation visuelle ou la combinaison de sources géographiques nécessite ainsi de récupérer de manière cohérente des données issues de plusieurs producteurs (IGN et Insee a minima) ce qui peut introduire des erreurs ou des incohérences dans des traitements automatisés.  
L’exploitation de données géographiques est particulièrement complexe lorsqu’on veut étudier des territoires sur plusieurs années – les fusions/séparations de commune impliquant de nombreuses difficultés – ou à différentes échelles – les découpages des villes divisées en arrondissements n’étant, par exemple, inclus dans le même shapefile que les découpages communaux alors que certaines sources de données les diffusent dans le même fichier.
 
Chaque institution développe ses propres codes de récupération de données ou entrepôts de contours géographiques à façon. Une mise en commun de ce patrimoine de code et de savoir serait bénéfique pour harmoniser cet écosystème foisonnant et permettre un accès facilité à des données fiables, normalisées et répondant aux besoins des analystes de données géographiques dont les niveaux de technicité varient. Faciliter un accès à des contours géographiques prêts à l’emploi pour des utilisateurs de données sous la forme d’API ou de catalogue de shapefiles serait très utile à des chercheurs, à des data-journalistes et aux différentes administrations qui produisent ou valorisent des données en open-data. Au-delà de ces publics, l’ensemble de l’écosystème de la data science qui utilise des données publiques pourrait trouver des gains à une exploitation facilitée des données géographiques.
 
 
#### Exemples de cas d'usage:
 
* Projet de cartographie de données
* Projet impliquant le croisement des données géographiques de l’Insee et de data.gouv.fr
 
#### Les objectifs :
 
* Rassembler données géographiques de l’IGN et administratives de l’INSEE dans un point d’entrée clair et normalisé (catalogue)
* Standardisation de données
* Développement d'API de mise à disposition des données
* Construction de shapefiles de confiance afin d'améliorer l’utilisation des données géographiques (éventuellement requêtables par API).
* Enjeu d’harmonisation avec l'écosystème existant: geofla, API découpage administratif, forum géocommun, avoir des retours de géomaticiens pour éviter de réinventer l'existant.
 
#### Les profils recherchés
 
* Data scientist
* Data Engineer
* Géomaticien
* Développeur