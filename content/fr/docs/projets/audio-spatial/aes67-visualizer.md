---
title: "aes67_visualizer"
weight: 7
description: "Visualiseur et moniteur de flux audio AES67 / ST2110-30 / RAVENNA / Dante — application desktop cross-platform"
tags: ["aes67", "ravenna", "dante", "st2110", "aoip", "electron", "react"]
---

{{< repo-card repo="aes67_visualizer" lang="true" >}}

## Présentation

Application desktop cross-platform de **visualisation et monitoring des flux audio-over-IP** : AES67, ST2110-30, RAVENNA et Dante. Détection automatique des flux sur le réseau, écoute, mesure de niveaux et suivi PTP.

## Fonctionnalités

- Découverte automatique des flux via **SAP/mDNS**
- Ajout manuel de flux par collage de SDP
- Interrogation directe des devices Dante via **ARC** (nom, modèle, canaux TX/RX)
- **Mur de monitoring** 16 slots en drag-and-drop
- Mesure de niveau **dBFS** temps réel avec peak hold
- Écoute de n'importe quel flux avec sélection de canal
- Suivi **PTP** (grandmaster IEEE 1588, statut de verrouillage par flux)
- Interface en **8 langues**
- Windows, macOS, Linux

## Stack technique

React 19 + TypeScript + Vite + TailwindCSS, desktop **Electron**, audio via Audify (bindings RtAudio).

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/aes67_visualizer)
