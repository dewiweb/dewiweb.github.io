---
title: "DewiCom"
weight: 6
description: "Local WiFi intercom for stage technicians — multi-channel PTT, zero install, zero cloud"
tags: ["intercom", "ptt", "wifi", "live-events", "nodejs", "electron", "android"]
---

{{< repo-card repo="dewicom" lang="true" >}}

## Overview

**Local WiFi intercom for stage technicians** — a multi-channel Push-To-Talk app: zero installation, zero cloud, zero subscription. All communications run over HTTPS/WSS (self-signed certificate generated at startup) to guarantee microphone access on every device.

## Architecture — 3 deployment levels

- **Standalone Node.js server** (Docker / dedicated) — level 1
- **Desktop app** Electron (Linux AppImage / Windows EXE)
- **Android app** (APK)
- Automatic failover between levels

## Features

- Multi-channel PTT over LAN
- Web UI shared across server, desktop and mobile
- Monitoring panel
- No external dependency

## Links

- [GitHub repository](https://github.com/dewiweb/dewicom)
