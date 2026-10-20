---
title: "Refonte du site et nouveaux projets documentés"
date: 2026-10-20
description: "Migration vers le thème Hextra et documentation d'une dizaine de projets récents"
tags: ["site", "hugo"]
---

Première note de ce carnet, à l'occasion d'une refonte complète du site.

## Le site

Le site tourne désormais sous **Hugo + thème Hextra**, avec :

- version bilingue **FR/EN**
- thème sombre par défaut, recherche intégrée
- lien **« Modifier cette page »** sur chaque page, qui mène directement au fichier source sur GitHub
- déploiement GitHub Pages via GitHub Actions, avec vérification de build sur les pull requests

## Nouvelles pages projets

La refonte s'accompagne de la documentation d'une dizaine de dépôts actifs qui n'étaient pas encore référencés :

- **[StageNeth](/docs/projets/outils-sceniques/stageneth/)** — OS pour routeur basé OpenWrt, dédié au spectacle vivant (VLANs AV, PTP, Dante/AES67/ST 2110)
- **[aes67_visualizer](/docs/projets/audio-spatial/aes67-visualizer/)** — visualiseur de flux AoIP (AES67, RAVENNA, Dante, ST 2110-30)
- **[ptp-monitor](/docs/projets/audio-spatial/ptp-monitor/)** — écoute passive des horloges PTP pour le diagnostic réseau AoIP
- **[DewiCom](/docs/projets/outils-sceniques/dewicom/)** — intercom WiFi PTT en réseau local pour techniciens
- **[audio-accessibility-system](/docs/projets/outils-sceniques/audio-accessibility-system/)** — diffusion audiodescription / renforcement audio via PWA
- **[nextevents](/docs/projets/outils-sceniques/nextevents/)** & **[openagenda-slides](/docs/projets/outils-sceniques/openagenda-slides/)** — diaporamas d'événements OpenAgenda pour affichage dynamique
- **[holophonix-animator-blender](/docs/projets/audio-spatial/holophonix-animator-blender/)** — animations Holophonix en addon Blender natif
- **[clock_X_overlay](/docs/projets/outils-sceniques/clock-x-overlay/)** — horloge OSD always-on-top pour Linux X11
- **[fooyin-album-mosaic-plugin](/docs/projets/outils-sceniques/fooyin-album-mosaic/)** — mosaïque de pochettes animée pour Fooyin
- module Companion **[oppo-bdp](/docs/projets/outils-sceniques/companion-modules/)** ajouté à la page des modules

La suite : des notes techniques au fil des projets — retours d'expérience, architectures, pièges rencontrés.
