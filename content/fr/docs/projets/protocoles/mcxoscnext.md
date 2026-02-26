---
title: "MCxOSCnext"
weight: 4
description: "Microservice web bridge Ember+ ↔ OSC — architecture Docker, backend Node.js + frontend React"
tags: ["ember+", "osc", "lawo", "riedel", "docker", "typescript", "broadcast"]
---

{{< repo-card repo="MCxOSCnext" lang="true" license="true" >}}

## Présentation

**MCxOSCnext** est la refonte complète de MCxOSC — passé d'une application Electron desktop à un **microservice web** déployable via Docker. Il fait le pont entre les équipements **Ember+** (consoles LAWO MC², matrices Riedel MediorNet...) et des systèmes de contrôle **OSC** (QLab, Chataigne, Max/MSP...).

```
┌─────────────┐     ┌──────────────────────────┐     ┌─────────────┐
│  Ember+     │◄───►│       MCxOSC Bridge       │◄───►│     OSC     │
│  (LAWO MC²) │ TCP │  Backend :3000  UI :80    │ UDP │  (QLab...)  │
└─────────────┘     └──────────────────────────┘     └─────────────┘
```

## Architecture

Le projet est organisé en monorepo avec deux packages :

- **Backend** (`Node.js / TypeScript`) — gestion Ember+, moteur OSC, API REST, WebSocket
- **Frontend** (`React / Vite`) — interface web de configuration et monitoring

## Fonctionnalités

- Bridge bidirectionnel **Ember+ ↔ OSC** en temps réel
- Interface web de configuration (IP, ports, mappings)
- Explorateur d'arbre Ember+ intégré
- Système de **sessions** — sauvegarde/rechargement des mappings
- API REST complète + WebSocket pour intégrations tierces
- **Vue matrice** pour les routeurs Ember+
- Déploiement **Docker** (one-liner, Compose, Portainer)
- Compatible LAWO MC², Riedel MediorNet, et tout device Ember+

## Démarrage rapide

```bash
# Déploiement one-liner sans cloner
curl -fsSL https://raw.githubusercontent.com/dewiweb/MCxOSCnext/develop/docker-compose.yml | \
  EMBER_HOST=192.168.1.100 docker compose -f - up -d
```

Accéder à l'interface : `http://localhost`

## Statut

⭐ **4 étoiles** · actif · v2.2.0-beta

## Liens

- [Dépôt GitHub](https://github.com/dewiweb/MCxOSCnext)
- [MCxOSC (version originale archivée)](https://github.com/dewiweb/MCxOSC)
