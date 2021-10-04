---
title: Classification des données de caisse dans des nomenclatures
summary: An example of using the in-built project page.
tags:
- Nouvelle source
- Codification
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

Les données de caisse donnent pour chaque code-barres (ou GTIN), chaque jour et chaque point de ventes les quantités vendues ainsi que le chiffre d’affaires et/ou le prix auquel le produit est vendu. Pour exploiter ces données, il est toutefois nécessaire de savoir quel produit se trouve derrière un code-barres. Actuellement, l’IPC se fonde sur un référentiel de codes-barres, acheté à un prestataire et qui donne une information très détaillée et structurée des caractéristiques de ces produits. Cette information est payante et ne couvre pas l’ensemble des produits. L’expérimentation vise à identifier les étapes de traitement textuel des libellés, ainsi que les méthodes de classification ou autres, permettant de coder automatiquement les libellés, sans passer par le référentiel, dans la nomenclature Coicop pour l’IPC et sur les regroupements utilisés pour Emagsa dans le cadre du projet Nosica qui vise à intégrer notamment les données de caisse dans la production des indicateurs d'activité de court-terme. Elle testera aussi leur performance sur des jeux de données tests. La division IPC ayant déjà classé les codes-barres dans la nomenclature Coicop grâce au référentiel de codes-barres, fournira des jeux de données d’apprentissage et de test pour entraîner et évaluer les performances des algorithmes et évaluer la pertinence des résultats de l’expérimentation. 
