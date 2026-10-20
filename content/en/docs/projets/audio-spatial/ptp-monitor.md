---
title: "ptp-monitor"
weight: 8
description: "Passive PTP clock monitoring for AoIP networks — Dante (PTPv1) and AES67/RAVENNA (PTPv2)"
tags: ["ptp", "aes67", "dante", "ravenna", "aoip", "python", "qt"]
---

{{< repo-card repo="ptp-monitor" lang="true" license="true" >}}

## Overview

Desktop tool (Qt / PySide6) for **passively listening to PTP clock traffic** on a production audio-over-IP network — to detect problems and record evidence for vendor support cases.

**100% passive**: it joins the standard PTP multicast group `224.0.1.129` (UDP 319/320) and listens. It never sends a single PTP packet and cannot disturb the clock election or timing of the network.

## Features

- **Dante leader (PTPv1)** — who sends Sync, sync interval, jitter (mean/min/max/σ), leader change history
- **AES67 grandmaster (PTPv2)** — clock identity, priorities, clock class, steps removed, announce timing
- **Per-source stats** — message types, rates, sequence gaps/dupes, silence detection, non-standard PTP domains
- **Malformed packets** — unparsable datagrams logged with source IP and full hexdump
- **Evidence logs** — chronological JSONL journal + optional full packet capture
- **Network-agnostic** — no hard-coded addresses; friendly device names via `devices.json`, reverse DNS and the IEEE OUI database

## Links

- [GitHub repository](https://github.com/dewiweb/ptp-monitor)
- Language: Python (Qt / PySide6)

> The UI is currently in French — i18n contributions are welcome.
