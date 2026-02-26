---
title: "spacemouse-osc"
linkTitle: "spacemouse-osc"
weight: 2
description: "Contrôleur 3D SpaceMouse vers OSC pour la spatialisation sonore"
tags: ["osc", "spacemouse", "3dconnexion", "audio-spatial", "javascript"]
---

{{< repo-card repo="spacemouse-osc" lang="true" license="true" >}}

## Présentation

Passerelle entre la **SpaceMouse Compact de 3Dconnexion** et le protocole **OSC** (Open Sound Control). Permet d'utiliser le contrôleur 6DoF (6 degrés de liberté) pour piloter des sources sonores dans l'espace 3D en temps réel.

Particulièrement adapté au contrôle de systèmes de spatialisation comme Holophonix, Max/MSP ou SuperCollider.

## Fonctionnalités

- Lecture des données 6DoF (translation X/Y/Z + rotation) de la SpaceMouse
- Conversion et envoi des données en messages OSC
- Mappages configurables (axes, adresses OSC, plages de valeurs)
- Faible latence pour le contrôle en temps réel

## Statut

⭐ **14 étoiles** · 1 fork · actif

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/spacemouse-osc)
- Langage : JavaScript
- Licence : MIT
- Topics : `3dconnexion` `6dof` `osc` `spacemouse` `spatial-audio`
