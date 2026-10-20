---
title: "aes67_visualizer"
weight: 7
description: "AES67 / ST2110-30 / RAVENNA / Dante audio stream visualizer and monitor — cross-platform desktop app"
tags: ["aes67", "ravenna", "dante", "st2110", "aoip", "electron", "react"]
---

{{< repo-card repo="aes67_visualizer" lang="true" >}}

## Overview

Cross-platform desktop application for **visualizing and monitoring audio-over-IP streams**: AES67, ST2110-30, RAVENNA and Dante. Automatic stream discovery on the network, playback, level metering and PTP tracking.

## Features

- Automatic stream discovery via **SAP/mDNS**
- Manual stream entry by pasting SDP
- Direct Dante device queries via **ARC** (name, model, TX/RX channels)
- **16-slot monitoring wall** with drag-and-drop
- Real-time **dBFS** metering with peak hold
- Listen to any stream with channel selection
- **PTP** tracking (IEEE 1588 grandmaster, per-stream lock status)
- UI in **8 languages**
- Windows, macOS, Linux

## Tech stack

React 19 + TypeScript + Vite + TailwindCSS, **Electron** desktop shell, audio via Audify (RtAudio bindings).

## Links

- [GitHub repository](https://github.com/dewiweb/aes67_visualizer)
