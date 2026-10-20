---
title: "audio-accessibility-system"
weight: 7
description: "Diffusion audio multicanal DIY pour salles de spectacle — audiodescription, renforcement audio, interprétation simultanée"
tags: ["accessibilité", "audiodescription", "aes67", "hls", "pwa", "docker"]
---

{{< repo-card repo="audio-accessibility-system" lang="true" >}}

## Présentation

Système de **diffusion audio multicanal DIY** pour salles de spectacle, de conférence et de cinéma (~450 places), conçu pour l'**audiodescription**, le **renforcement audio** (malentendants) et l'**interprétation simultanée multilingue**.

La source audio arrive en **AES67/RTP** depuis la console son, est encodée en **HLS** par FFmpeg et servie aux smartphones des spectateurs via une **PWA** — aucune app à installer.

## Fonctionnalités

- Backend Node.js + streaming HLS (HTTPS/TLS)
- Réception AES67/RTP multicast (L24/48 kHz) depuis consoles QSYS/Dante
- Interface auditeur PWA + interface admin régie
- Sécurité (JWT, CSP, bcrypt), déploiement Docker/Portainer
- CI/CD GitHub Actions → GHCR (amd64 + arm64)

## Statut

✅ Opérationnel — tests en conditions réelles (450 clients) en cours ; WebRTC (< 200 ms) prévu pour réduire la latence.

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/audio-accessibility-system)
