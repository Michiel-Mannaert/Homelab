# Homelab Architecture Overview

## Introduction
This homelab consists of 4 Proxmox nodes designed to simulate a small enterprise infrastructure environment.

---

## Infrastructure Nodes

| Node | Name   | Role |
|------|--------|------|
| Node 1 | Kenobi | Core Infrastructure |
| Node 2 | Anakin | Security & Pentesting |
| Node 3 | Yoda   | Storage & Backups |
| Node 4 | Maul   | Kubernetes & Experiments |

---

## Design Principles

- Separation of concerns
- Isolation of security workloads
- Dedicated storage layer
- Experimental workloads isolated
- Production-like core infrastructure

---

## Main Services

- Active Directory (Windows Server)
- DNS / DHCP
- Docker services stack
- Kubernetes cluster (k3s)
- Security lab (SIEM + pentesting tools)
- Backup infrastructure (Proxmox Backup + NAS)

---

## Network Design

- VLAN segmentation
- pfSense firewall routing
- Internal management network
- Isolated security network
- Kubernetes network segment