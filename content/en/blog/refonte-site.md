---
title: "Site rebuild and newly documented projects"
date: 2026-10-20
description: "Migration to the Hextra theme and documentation of ten recent projects"
tags: ["site", "hugo"]
---

First entry in this notebook, on the occasion of a full site rebuild.

## The site

The site now runs on **Hugo + the Hextra theme**, with:

- a bilingual **FR/EN** version
- dark theme by default, built-in search
- an **"Edit this page"** link on every page leading straight to the source file on GitHub
- GitHub Pages deployment via GitHub Actions, with a build check on pull requests

## New project pages

The rebuild comes with documentation for about ten active repositories that weren't listed yet:

- **[StageNeth](/en/docs/projets/outils-sceniques/stageneth/)** — OpenWrt-based router OS for live performance (AV VLANs, PTP, Dante/AES67/ST 2110)
- **[aes67_visualizer](/en/docs/projets/audio-spatial/aes67-visualizer/)** — AoIP stream visualizer (AES67, RAVENNA, Dante, ST 2110-30)
- **[ptp-monitor](/en/docs/projets/audio-spatial/ptp-monitor/)** — passive PTP clock listening for AoIP network diagnostics
- **[DewiCom](/en/docs/projets/outils-sceniques/dewicom/)** — local WiFi PTT intercom for stage technicians
- **[audio-accessibility-system](/en/docs/projets/outils-sceniques/audio-accessibility-system/)** — audio description / hearing assistance distribution via PWA
- **[nextevents](/en/docs/projets/outils-sceniques/nextevents/)** & **[openagenda-slides](/en/docs/projets/outils-sceniques/openagenda-slides/)** — OpenAgenda event slideshows for digital signage
- **[holophonix-animator-blender](/en/docs/projets/audio-spatial/holophonix-animator-blender/)** — Holophonix animations as a native Blender addon
- **[clock_X_overlay](/en/docs/projets/outils-sceniques/clock-x-overlay/)** — always-on-top OSD clock for Linux X11
- **[fooyin-album-mosaic-plugin](/en/docs/projets/outils-sceniques/fooyin-album-mosaic/)** — animated album-cover mosaic for Fooyin
- the **[oppo-bdp](/en/docs/projets/outils-sceniques/companion-modules/)** Companion module added to the modules page

Next up: technical notes as projects evolve — lessons learned, architectures, pitfalls.
