---
title: "MCxOSCnext"
weight: 4
description: "Web microservice bridging Ember+ ↔ OSC — Docker, Node.js backend + React frontend"
tags: ["ember+", "osc", "lawo", "riedel", "docker", "typescript", "broadcast"]
---

{{< repo-card repo="MCxOSCnext" lang="true" license="true" >}}

## Overview

**MCxOSCnext** is a full rewrite of MCxOSC — evolved from a desktop Electron app into a **web microservice** deployable via Docker. It bridges **Ember+** devices (LAWO MC² consoles, Riedel MediorNet matrices...) with **OSC** control systems (QLab, Chataigne, Max/MSP...).

```
┌─────────────┐     ┌──────────────────────────┐     ┌─────────────┐
│  Ember+     │◄───►│       MCxOSC Bridge       │◄───►│     OSC     │
│  (LAWO MC²) │ TCP │  Backend :3000  UI :80    │ UDP │  (QLab...)  │
└─────────────┘     └──────────────────────────┘     └─────────────┘
```

## Architecture

Monorepo with two packages:

- **Backend** (`Node.js / TypeScript`) — Ember+ engine, OSC engine, REST API, WebSocket
- **Frontend** (`React / Vite`) — web UI for configuration and monitoring

## Features

- Bidirectional **Ember+ ↔ OSC** bridge in real time
- Web UI for device configuration (IP, ports, mappings)
- Built-in Ember+ tree explorer
- **Session** system — save and reload connection mappings
- Full REST API + WebSocket for third-party integrations
- **Matrix view** for Ember+ routers
- **Docker** deployment (one-liner, Compose, Portainer)
- Compatible with LAWO MC², Riedel MediorNet, and any Ember+ device

## Quick start

```bash
# One-liner deployment — no cloning required
curl -fsSL https://raw.githubusercontent.com/dewiweb/MCxOSCnext/develop/docker-compose.yml | \
  EMBER_HOST=192.168.1.100 docker compose -f - up -d
```

Open the UI at `http://localhost`

## Status

⭐ **4 stars** · active · v2.2.0-beta

## Links

- [GitHub repository](https://github.com/dewiweb/MCxOSCnext)
- [MCxOSC (original archived version)](https://github.com/dewiweb/MCxOSC)
