---
title: "ptp-monitor"
weight: 8
description: "Monitoring passif des horloges PTP pour réseaux AoIP — Dante (PTPv1) et AES67/RAVENNA (PTPv2)"
tags: ["ptp", "aes67", "dante", "ravenna", "aoip", "python", "qt"]
---

{{< repo-card repo="ptp-monitor" lang="true" license="true" >}}

## Présentation

Outil desktop (Qt / PySide6) d'**écoute passive du trafic d'horloge PTP** sur un réseau audio-over-IP de production — pour détecter les problèmes et constituer des preuves à transmettre au support constructeur.

**100 % passif** : rejoint le groupe multicast standard `224.0.1.129` (UDP 319/320) et écoute. Aucun paquet émis, aucune perturbation possible de l'élection d'horloge.

## Fonctionnalités

- **Leader Dante (PTPv1)** — émetteur des Sync, intervalle, jitter (moyenne/min/max/σ), historique des changements de leader
- **Grandmaster AES67 (PTPv2)** — identité d'horloge, priorités, clock class, steps removed, cadence des Announce
- **Stats par source** — types de messages, débits, trous/doublons de séquence, détection de silence, domaines PTP non standard
- **Paquets malformés** — datagrammes imparsables journalisés avec IP source et hexdump complet
- **Journaux de preuve** — journal chronologique JSONL + capture complète optionnelle
- **Agnostique réseau** — aucune adresse codée en dur ; noms d'équipements via `devices.json`, DNS inverse et base OUI IEEE

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/ptp-monitor)
- Langage : Python (Qt / PySide6)

> L'interface est actuellement en français — les contributions i18n sont bienvenues.
