---
title: "StageNeth"
weight: 5
description: "OS pour routeur dédié au spectacle vivant basé sur OpenWrt — séparation des flux AV, PTP, services réseau scéniques"
tags: ["openwrt", "réseau", "dante", "aes67", "st2110", "ndi", "ptp", "go", "vue"]
---

{{< repo-card repo="stageneth" lang="true" >}}

## Présentation

**OS pour routeur dédié au spectacle vivant**, basé sur **OpenWrt**. StageNeth sépare les flux audio/vidéo/lumière (AV) du réseau de gestion et fournit les services indispensables aux équipements scéniques : DHCP, NTP, mDNS, SNMP et PTP.

## Fonctionnalités

- **Interface web Vue 3** en HTTPS — mode simple (opérateur) et mode expert (tech)
- **API Go** sécurisée (sessions HttpOnly, mots de passe argon2id, rôles opérateur/tech)
- **Orchestrateur réseau Go** — génération automatique des VLANs 802.1q, bridges, firewall, DHCP, QoS/NIC tuning et PTP
- **Configuration par service** — chaque protocole (Dante, NDI, AES67/RAVENNA, ST 2110, Art-Net, sACN, PTP, AVB, NMOS, MA-Net…) a son VLAN, son DSCP, sa priorité et son MTU
- Trunk AV configurable et interface dédiée ST 2110 en jumbo frames (MTU 9000)
- Serveur NTP avec option DHCP 42 par VLAN, réflecteur mDNS entre VLANs AV
- Surveillance : monitoring CPU/mémoire/services, alertes, journaux filtrés, agent SNMP v2c/v3, métriques Prometheus

## Statut

🚧 **Développement actif** (v0.2.0-beta) — à valider sur banc avant tout usage en production.

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/stageneth)
- Langages : Go, Vue 3, OpenWrt
