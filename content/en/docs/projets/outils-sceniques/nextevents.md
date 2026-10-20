---
title: "nextevents"
weight: 8
description: "OpenAgenda event slideshow suite for Les Champs Libres — Docker server, portable desktop app and PHP port"
tags: ["openagenda", "digital-signage", "champs-libres", "python", "qt", "php", "docker"]
---

{{< repo-card repo="nextevents" lang="true" >}}

## Overview

A suite of tools generating **slideshows of Les Champs Libres events** (Rennes, France) from OpenAgenda data — UHD slides ready for OBS, digital signage and kiosks.

Three variants depending on the infrastructure:

- **[nextevents](https://github.com/dewiweb/nextevents)** — Debian/Docker server: scrapes leschampslibres.fr + OpenAgenda, renders **UHD 3840×2160** PNGs matching the venue's visual identity (Oldschool Grotesk typeface, per-event pastel background), web UI with gallery and auto-refresh
- **[nextevents-desktop](https://github.com/dewiweb/nextevents-desktop)** — rewritten as a **portable PySide6/Qt app** (Windows zip, Linux AppImage): same slide generation plus a native fullscreen player, no Docker or server needed
- **[nextevents-php](https://github.com/dewiweb/nextevents-php)** — lightweight PHP port for kiosks: self-contained HTML slides (fonts/images in base64), no PNG generation, no dependencies — the kiosk browser does the rendering

## Common features

- Date, duration, venue, price, **audience** and **accessibility** (LSF, audio description, surtitling) extracted from OpenAgenda data
- Native-resolution images, FTP/SMB/local sync
- Slide of the day, scheduler, gallery

## Links

- [nextevents](https://github.com/dewiweb/nextevents) · [nextevents-desktop](https://github.com/dewiweb/nextevents-desktop) · [nextevents-php](https://github.com/dewiweb/nextevents-php)
- See also [openagenda-slides](/en/docs/projets/outils-sceniques/openagenda-slides/) — the generalized version for any public OpenAgenda agenda
