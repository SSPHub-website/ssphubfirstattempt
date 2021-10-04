---
title: Webscraping du prix et des caractéristiques des ordinateurs portables
summary: Estimation de modèles hédoniques pour améliorer la qualité statistique de l’indice des prix à la consommation
tags:
- Webscrapping
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

L’indice des prix à la consommation (IPC) est l’indicateur mesurant l’inflation en France. Cet indicea un rôle très important dans l’économie: outre son impact sur la politique monétaire, il est utilisépour l’indexation de contrats privés, de pensions alimentaires, pour la revalorisation du SMIC, desretraites et des loyers, dans des instruments financiers, etc.L’IPC mesure, chaque mois, l’évolution «pure» des prix, à qualité constante. Ainsi, il s’agit desuivre un certain nombre de produits identiques dans le temps. Lorsque ceux-ci disparaissent, ilssont   remplacés  par des  produits qui   peuvent   ne pas  être  équivalents.  Il  convient   alors  dedistinguer, dans l’évolution des prix des remplaçants par rapport aux produits remplacés, un effetqualité (différence de prix pour un mois fixé), de l’effet inflation que l’on cherche à mesurer.Certaines méthodes, dites «hédoniques», consistent à estimer cet effet qualité à partir decoefficients correspondant aux prix sous-jacents des différentes caractéristiques techniques duproduit (par exemple la marque de l’ordinateur, la mémoire vive d’un ordinateur, le modèle et lafréquence du processeur, etc.). Cette estimation est typiquement réalisée par des modèles derégression. On recourt aujourd’hui à ce type de méthodes pour seulement quatre types de produitsaujourd’hui dans l’IPC, mais la qualité statistique des estimations est faible, notamment à caused’un nombre de prix relevés trop faible. Le recours au Webscraping des caractéristiques et desprix des produits offre l’opportunité d’augmenter significativement le nombre de relevés de prix etde caractéristiques des produits. Le but de l’expérimentation est donc de revoir les estimations etles modèles de prix hédoniques au vu des nouvelles données scrapées pour les produits pourlesquels les modèles hédoniques sont déjà utilisés et d’étendre le recours à ces méthodes àd’autres produits (en particulier des biens électroniques: smartphones, ordinateurs, tablettes, etc.).Les données collectées sur Internet par webscraping forment des ensembles d’estimation assezlarges pour envisager des sélections de modèles et des modèles de régression pénalisée (de typeLasso) où le nombre de variables explicatives (caractéristiques) est très grand afin d’estimer l’effetqualité correspondant à chaque caractéristique. Les résultats obtenus permettront d’envisager uneimplémentation dans l’IPC, et ainsi une amélioration statistique de l’estimation de l’inflation enFrance. Des   travaux   exploratoires   seront   également   menés,   sur   la   pertinence   d’autres   modèles   deprédiction   des   prix:   random   forests,   bagging,   boosting,   etc.,   à   partir   des   caractéristiquestechniques) machine learning, etc.
