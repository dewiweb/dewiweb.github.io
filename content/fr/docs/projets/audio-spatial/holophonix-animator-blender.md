---
title: "holophonix-animator-blender"
weight: 9
description: "Addon Blender natif pour animer les pistes Holophonix — modèles de mouvement, cue list, sortie OSC temps réel"
tags: ["holophonix", "blender", "audio-spatial", "osc", "python"]
---

{{< repo-card repo="holophonix-animator-blender" lang="true" >}}

## Présentation

Portage de **holophonix-animator** en **addon Blender natif** : créer et jouer des animations de mouvement pour les pistes audio spatiales Holophonix directement dans la 3D View de Blender. Complète [holophonix_blender_addon](/docs/projets/audio-spatial/holophonix-blender-addon/), orienté gestion de projets.

## Fonctionnalités

- Import de projets Holophonix (`.hol`, `.zip`)
- Découverte des pistes via requête OSC `/dump`
- Animation **temps réel** (modes loop / ping-pong / once)
- **Animations simultanées** — chaque piste indépendante
- **Cue list** — déclenchement, arrêt, fondu entre animations
- Modèles de mouvement (JSON extensible) : circulaire, linéaire, figure-8, spirale, pendule, marche aléatoire
- Sortie **OSC** `/track/{id}/xyz` en temps réel pendant la lecture

## Prérequis

- Blender 4.2+ (testé sur 5.0)
- Libs OSC embarquées — aucune installation externe

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/holophonix-animator-blender)
- Langage : Python
