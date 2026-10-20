---
title: "StageNeth"
weight: 5
description: "Router OS for live performance environments based on OpenWrt — AV stream separation, PTP, stage network services"
tags: ["openwrt", "network", "dante", "aes67", "st2110", "ndi", "ptp", "go", "vue"]
---

{{< repo-card repo="stageneth" lang="true" >}}

## Overview

**Router OS designed for live performance environments**, based on **OpenWrt**. StageNeth separates audio/video/lighting (AV) streams from the management network and provides the services stage equipment relies on: DHCP, NTP, mDNS, SNMP and PTP.

## Features

- **Vue 3 web UI** over HTTPS — simple mode (operator) and expert mode (tech)
- **Secured Go API** (HttpOnly sessions, argon2id passwords, operator/tech roles)
- **Go network orchestrator** — automatic generation of 802.1q VLANs, bridges, firewall, DHCP, QoS/NIC tuning and PTP
- **Per-service configuration** — each protocol (Dante, NDI, AES67/RAVENNA, ST 2110, Art-Net, sACN, PTP, AVB, NMOS, MA-Net…) gets its own VLAN, DSCP, priority and MTU
- Configurable AV trunk and dedicated ST 2110 interface with jumbo frames (MTU 9000)
- NTP server with DHCP option 42 per VLAN, mDNS reflector across AV VLANs
- Monitoring: CPU/memory/services, alerts, filterable logs, SNMP v2c/v3 agent, Prometheus metrics

## Status

🚧 **Active development** (v0.2.0-beta) — validate on the bench before any production use.

## Links

- [GitHub repository](https://github.com/dewiweb/stageneth)
- Languages: Go, Vue 3, OpenWrt
