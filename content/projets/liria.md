---
title: "OCR et extraction d'informations à partir de documents administratifs"
summary: Les administrations ont régulièrement besoin d’exploiter en masse des documents administratifs sous des formats non directement exploitables (PDF scannés, images, etc.). L’information contenue dans ces documents, pour être exploitée, doit passer par une étape d'extraction et de structuration de l’information, qui est vite très chronophage si elle doit être réalisée à la main.
responsible: Kim Montalibet (DINUM)
date: 2022-05-18T13:00:00+01:00
images: 
- /img/image-ocr.png
---

##### Les objectifs 
* Dans un premier temps, il s'agira de faire l'état des lieux des travaux déjà réalisés dans le domaine, de partager des retours sur les librairies testées et de centraliser ces éléments dans une documentation de tpe wiki. 
* Dans un 2eme temps, prioriser les cas d'usages identifiés et dévelepper des briques open source pour y répondre.

##### Exemples de cas d'usage
* PEREN : fournir des données structurées et comparables depuis des rapports de transparence publiés par les plateformes numériques (exemple : https://transparencyreport.google.com/report-downloads)
* Ministère des Armées: fiches de poste, rapports du Contrôle général des armées 
* Haute Autorité de la Santé: rapports des recommandations professionnelles (PDF numérisés): extraire des info afin de construire un arbre de décision
* INSEE : 
  * la numérisation de tickets de caisse collectés par l’enquête budget des familles
  * extraire les tableaux des comptes sociaux (données et API INPI). PDF scannés
* Services statistiques ministériels: nombreuses publications en format papier (numérisation puis structuration automatique des informations présentes dans ces publications pourraient permettre de publier ces données en open data afin de rendre possible des réutilisations par des chercheurs, data scientists) 
* La start-up d'Etat [Dossier Facile](https://www.dossierfacile.fr/) : OCR et extraction d'informations sur les cartes d'identités, bulletins de salaires et quittances de loyer 

##### Domaines techniques 
- OCR : de 3 types tapuscrit, manuscrit, tableau 
- Extraction d'informations, plusieurs problématiques : 
  - développer un outil d'extractions de données structurées depuis des fichiers PDF correctement formatés en s'appuyant sur le contexte afin de lier les informations entre elles et d'établir des hiérarchies.
  - développer un outil d'extraction à partir de documents contenant du texte et des éléments de mise en page ayant une importance (type carte d'identité, bulletins de salaires) 


##### Les profils recherchés
* Data scientist (compétences en NLP, computeur vision)
* Développeur 

##### Ressources utiles 
* [Repertoire GitHub du projet OCR-Xtract](https://github.com/etalab-ia/ocr-xtract )
* CORD, jeu de données de tickets de caisse, ouvert et annoté : https://github.com/clovaai/cord 
* Tutoriel pour l'utilisation de la librairie LayoutLM : https://github.com/omarsou/layoutlm_CORD/blob/main/layoutlm.ipynb 
* Rapports de transparence publiés par les plateformes numériques :  https://transparencyreport.google.com/report-downloads

