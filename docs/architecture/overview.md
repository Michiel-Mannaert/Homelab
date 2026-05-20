# Enterprise Homelab Architecture Overview

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

### Service Placement

- Active Directory → Node 1 (Kenobi)
- Docker Stack → Node 1 (Kenobi)
- Security Lab (Kali, Wazuh, etc.) → Node 2 (Anakin)
- Backup Infrastructure (Proxmox Backup, TrueNAS) → Node 3 (Yoda)
- Kubernetes Cluster (k3s) → Node 4 (Maul)

## Network Design

- VLAN segmentation
- pfSense firewall routing
- Internal management network
- Isolated security network
- Kubernetes network segment

## Purpose

This environment is built to replicate real-world enterprise infrastructure for learning:

- System administration
- Network engineering
- Cybersecurity (blue & red team)
- DevOps & automation
- Kubernetes orchestration