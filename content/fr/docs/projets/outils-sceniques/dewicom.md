---
title: "DewiCom"
weight: 6
description: "Intercom WiFi local pour techniciens scène — PTT multi-canal, zéro installation, zéro cloud"
tags: ["intercom", "ptt", "wifi", "spectacle", "nodejs", "electron", "android"]
---

{{< repo-card repo="dewicom" lang="true" >}}

## Présentation

**Intercom WiFi en réseau local pour techniciens scène** — application Push-To-Talk multi-canal : zéro installation, zéro cloud, zéro abonnement. Toutes les communications passent en HTTPS/WSS (certificat auto-signé généré au démarrage) pour garantir l'accès au microphone sur tous les appareils.

## Architecture — 3 niveaux de déploiement

- **Serveur Node.js** standalone (Docker / dédié) — niveau 1
- **Application desktop** Electron (AppImage Linux / EXE Windows)
- **Application mobile** Android (APK)
- Failover automatique entre les niveaux

## Fonctionnalités

- PTT multi-canal sur le réseau local
- Interface web partagée entre serveur, desktop et mobile
- Panneau de monitoring
- Aucune dépendance externe

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/dewicom)
