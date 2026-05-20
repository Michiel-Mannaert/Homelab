# Hardware Overview

## Proxmox Cluster

| Node | Role | CPU | RAM | Storage |
|------|------|-----|-----|---------|
| Kenobi | Core Infrastructure | 8 x Intel(R) Core(TM) i7-9700 CPU @ 3.00GHz (1 Socket) | 32 GB | sata SSD + VM Storage (nvme SSD) |
| Yoda | Security Lab | 6 x Intel(R) Core(TM) i5-9500T CPU @ 2.20GHz (1 Socket) | 16 GB | sata SSD + VM Storage (nvmd SSD) |
| Anakin | Storage | TBD | 16 GB | sata SSD + VM Storage (nvmd SSD)  |
| Maul | Kubernetes/experiments | TBD | 16 GB | sata SSD + VM Storage (nvmd SSD) |

---

## Design Notes

- Nodes are separated by function
- Storage is isolated from compute workloads/VM disks
- Security environment is fully separated
- RAM is upgradable in the future