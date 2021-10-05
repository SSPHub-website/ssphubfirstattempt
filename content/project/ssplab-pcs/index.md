---
title: Codification automatique des professions dans la nomenclature PCS 2020
summary: 
tags:
- Classification
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

La rénovation de la nomenclature des PCS en 2020 s'accompagne de la promotion d'un outil d'autocomplétion des libellés de profession dans une liste de libellés enrichis permettant le codage direct dans la case de la nomenclature ou des regroupements ad hoc complémentaires de la nomenclature. Or, l'outil d'autocomplétion ne sera disponible que pour des collectes informatisées et par ailleurs il comprend la possibilité de répondre "hors-liste". Pour pouvoir intégrer la nouvelle PCS 2020 dans le recensement de population à la collecte 2024 et être en mesure de coder aussi les bulletins papier tout comme les réponses informatisées "hors-liste", un algorithme de codification automatique en PCS 2020 de ces bulletins doit être créé. Suite au report de l'enquête de rencensement 2021, des gestionnaires ont annoté en PCS 2020, avec double codage et arbitrage, 119 000 bulletins issus de l'EAR 2020. Le but de l'expérimentation est de tester et comparer différents modèles d'apprentissage statistique et méthodes de prétraitement pour le codage des professions dans la nomenclature PCS 2020 à partir du libellé de profession ainsi que des variables annexes utilisées lors de la phase d'annotation (statut de l'employeur, etc.) et d'en retenir le plus performant. L'objectif est de maintenir le taux de codifications correctes ainsi que le taux d'envoi en reprise manuelle à des niveaux similaires à l'existant.

{{% staticref "uploads/fiche_experimentation_PCS.pdf" "newtab" %}}La description de cette expérimentation a par ailleurs fait l'objet d'une note d'intention{{% /staticref %}}


