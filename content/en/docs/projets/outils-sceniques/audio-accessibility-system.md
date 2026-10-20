---
title: "audio-accessibility-system"
weight: 7
description: "DIY multichannel audio distribution for venues — audio description, hearing assistance, simultaneous interpretation"
tags: ["accessibility", "audio-description", "aes67", "hls", "pwa", "docker"]
---

{{< repo-card repo="audio-accessibility-system" lang="true" >}}

## Overview

**DIY multichannel audio distribution system** for theatres, conference halls and cinemas (~450 seats), designed for **audio description**, **hearing assistance** (hard-of-hearing audiences) and **multilingual simultaneous interpretation**.

Audio is received via **AES67/RTP** from the mixing console, encoded to **HLS** by FFmpeg and served to audience smartphones through a **PWA** — no app to install.

## Features

- Node.js backend + HLS streaming (HTTPS/TLS)
- AES67/RTP multicast input (L24/48 kHz) from QSYS/Dante consoles
- Listener PWA + control-room admin UI
- Security (JWT, CSP, bcrypt), Docker/Portainer deployment
- CI/CD GitHub Actions → GHCR (amd64 + arm64)

## Status

✅ Operational — real-world testing (450 clients) in progress; WebRTC (< 200 ms) planned to reduce latency.

## Links

- [GitHub repository](https://github.com/dewiweb/audio-accessibility-system)
