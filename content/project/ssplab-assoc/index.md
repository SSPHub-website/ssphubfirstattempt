---
title: Codage automatique de l'activité des associations à partir de méthodes de machine learning
summary: An example of using the in-built project page.
tags:
- Codification Automatique
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

L’enjeu de l’expérimentation est d’attribuer un domaine d’activité aux associations pour améliorer le tirage de l’échantillon de l’enquête associations. En effet, une partie des associations est répertoriée dans Sirène (employeuses, subventionnées…) mais 50 % d’entre elles ont un code APE 9499Z ne permettant pas de déterminer leur domaine d’activité de façon précise. Par ailleurs, les associations loi 1901 sont enregistrées dans le répertoire national des associations (RNA), géré par le ministère de l’intérieur. Dans ce répertoire, un champ "objet social" rempli en clair décrit rapidement les activités de chaque association. L’expérimentation vise à analyser textuellement ce champ pour en prédire l'activité. L'enquête 2014 appariée au RNA sert de jeu d'apprentissage et de jeu de tests. 

En production : l'échantillon de l'enquête Association 2019 a été tiré selon une stratification tirant profit de la prédiction du secteur d'activité par machine learning (XGboost) mené dans le cadre de cette expérimentation : note sur l'échantillonnage de l'enquête, présentation interne des résultats (slides). Les résultats approfondis sont disponibles dans le mémoire de master Evaluation et Décision Publiques, majeure méthodologie de la statistique publique de F Lécrivain (note d'étape, rapport). En pratique, après prétraitements et exploration des données textuelles et de ses thématiques (allocation latente de Dirichlet), un dictionnaire des mots a été constitué, avec des variantes pour en réduire la dimension (tf-idf, seuil, thèmes d’une LDA). La prédiction proprement dite s’est appuyée sur divers modèles d’apprentissage supervisé (forêts aléatoires, support vector machine, modèle linéaires généralisés pénalisés GLMnet et Extrem Gradient Boosting (XGBoost), le jeu d’apprentissage (et les jeux de tests) étant fournis par la précédente enquête (2014) appariée avec le RNA. Le modèle XGboost a montré des performances plus élevés que les autres (avec une précision et un rappel de l’ordre de 69%). Le meilleur modèle s’obtient en combinant les différents modèles testés.
