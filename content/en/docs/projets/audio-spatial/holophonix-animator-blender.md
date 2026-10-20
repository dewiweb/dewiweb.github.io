---
title: "holophonix-animator-blender"
weight: 9
description: "Native Blender addon to animate Holophonix spatial audio tracks — motion models, cue list, real-time OSC output"
tags: ["holophonix", "blender", "audio-spatial", "osc", "python"]
---

{{< repo-card repo="holophonix-animator-blender" lang="true" >}}

## Overview

Port of **holophonix-animator** as a **native Blender addon**: create and play motion animations for Holophonix spatial audio tracks directly inside Blender's 3D View. Complements [holophonix_blender_addon](/en/docs/projets/audio-spatial/holophonix-blender-addon/), which focuses on project management.

## Features

- Import Holophonix projects (`.hol`, `.zip`)
- Track discovery via OSC `/dump` request
- **Real-time** animation (loop / ping-pong / once modes)
- **Simultaneous animations** — each track runs independently
- **Cue list** — trigger, stop and blend animations on demand
- Motion models (extensible JSON): circular, linear, figure-8, spiral, pendulum, random walk
- **OSC** output `/track/{id}/xyz` in real time during playback

## Requirements

- Blender 4.2+ (tested on 5.0)
- OSC libs bundled — no external install needed

## Links

- [GitHub repository](https://github.com/dewiweb/holophonix-animator-blender)
- Language: Python
