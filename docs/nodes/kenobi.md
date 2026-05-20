# Node 1 — Kenobi

## Role
Core infrastructure node for stable services.

## Virtual Machines

- DC01 (Windows Server)
  - AD
  - DNS
  - DHCP
  - CA

## LXC containers
- Pi-hole
  - DNS
  - DHCP
  - Add-blocker

- Wireguard VPN


## Purpose
Stable always-on infrastructure services.

## Notes
No experimental workloads allowed.
Docker VM still to be made