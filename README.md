# NETFORGE — Network Topology Mapper

Visual network topology mapper and documentation tool. Drag and drop 20 device types onto a canvas, draw connections with 5 link types, manage VLANs and subnets, and export to JSON, Markdown, Mermaid diagrams, or CSV inventory. Supports both enterprise infrastructure and home lab devices. Single HTML file, zero dependencies.

## Live Demo

**[nexusfang-tech.github.io/netforge](https://nexusfang-tech.github.io/netforge/)**

## Device Types (20)

| Category | Devices |
|----------|---------|
| Network | Firewall, Router, Switch, Access Point |
| Servers | Server, Database, DNS Server, Domain Controller |
| Endpoints | Workstation, Mobile Device, Printer, IoT Device |
| Cloud & Tunnel | Cloud Service, VPN Gateway, Cloudflare Tunnel, CDN/Proxy |
| Home Lab | Proxmox Host, Pi-hole, Docker Host, NAS |

## Features

- **Drag-and-drop canvas** — Place devices from the sidebar, move freely with pan and zoom
- **Connection drawing** — Click ports on devices to create links with 5 types:
  - Ethernet (solid blue), Trunk (solid green), Wireless (dashed orange), VPN (solid purple), Logical (dashed gray)
- **Device properties** — Hostname, IP, MAC address, VLAN assignment, subnet, OS/firmware, services/ports, status (online/offline/warning), and notes
- **VLAN management** — Pre-loaded with 5 common VLANs (Management, Servers, Users, IoT, DMZ), add custom VLANs with auto-generated CIDR notation
- **Auto arrange** — Layer-based layout: Security → Network → Servers → Endpoints → Cloud
- **Demo topology** — Pre-built enterprise + home lab hybrid network (pfSense, VyOS, Cisco, UniFi, Proxmox, Pi-hole, Azure VM, Cloudflare Tunnel)
- **Save/Load** — Persist to browser localStorage
- **Minimap** — Overview of the full topology with device positions

## Export Formats

| Format | Description |
|--------|-------------|
| JSON | Full topology data, re-importable |
| Markdown | Table-formatted documentation for wikis or READMEs |
| Mermaid | Diagram markup with link type styling |
| CSV | Device inventory + connection list for spreadsheets |

## Tech Stack

Vanilla JavaScript · HTML Canvas · CSS · GitHub Pages

## Author

**Matt Keith** · [nexusfang-tech.github.io](https://nexusfang-tech.github.io)
