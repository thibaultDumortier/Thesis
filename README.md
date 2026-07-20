# Mémoire de Thibault DUMORTIER

## Sujet

Ce mémoire intitulé "Identification de fragments parallèles dans des corpus comparables pour les langues régionales de France"
étudie la question de l'identification de fragments étant une traduction 1:1 l'un de l'autre dans des corpus comparables (corpus ayant
un même sujet mais dont les documents ne sont pas des traductions directes d'un texte à l'autre) pour l'alsacien, l'occitan et le corse.

## Trouvable dans ce dépôt

Dans ce dépôt Git sont retrouvables :
- Le mémoire dans son entièreté sous forme d'un code LaTeX.
- Un programme d'analyse de données "data_analysis.py" permettant de connaître le nombre de tokens, phrases, etc. présents dans un corpus.
- Les différents notebooks utilisés au cours de la réalisation de ce mémoire.
  - Similarities_SBERT étant le notebook permettant de calculer la similarité sémantique avec SBERT pour les  différents documents du corpus avec
  établissement des paires de phrases FR-LR, le chargement des corpus parallèles (pas rendu disponible ici), la création des sous-ensembles
  pour chacune des classes (parallèles, semi-parallèles et non-parallèles). Ce notebook permet aussi le calcul des autres variables importantes
  dans ce mémoire.
  - Deux notebooks nommés Classifieur_regression_logistique_loads et Trained_models_classifieur_regression_logistique_exec. Respectivement le premier de ces
  notebooks permet la création du modèle binaire et multiclasse et de leur scaler. Le deuxième réutilise les modèles déjà compilés au format .joblib pour relancer des
  évaluations. Celui-ci était principalement utilisé lors du mémoire pour réutiliser les mêmes modèles sans avoir à les recompiler et sans changer leur fonctionnement interne.
  - Un notebook nommé validation_modele. Celui-ci réalise la validation des modèles sur un corpus comparable donné. Dans le cas de notre mémoire, ce corpus
  était basé sur Wikipédia et réalisé via un autre programme basé sur les travaux de P.TSOLAKIS(2023) non présent sur ce dépôt.
- Les modèles au format "joblib" et les CSV des paires provenant du corpus comparable Wikipédia.

## Auteur et license

Auteur : Thibault DUMORTIER
License : GNU GPLv3
