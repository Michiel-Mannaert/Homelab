# Hardware Overview

## Proxmox Cluster

| Node | Role | CPU | RAM | Storage |
|------|------|-----|-----|---------|
| Kenobi | Core Infrastructure | 8 x Intel(R) Core(TM) i7-9700 CPU @ 3.00GHz (1 Socket) | 32 GB | sata SSD + VM Storage (nvme SSD) |
| Yoda | Security Lab | 6 x Intel(R) Core(TM) i5-9500T CPU @ 2.20GHz (1 Socket) | 16 GB | sata SSD + VM Storage (nvmd SSD) |
| Anakin | Storage | TBD | TBD | HDD/RAID/ZFS |
| Maul | Kubernetes/experiments | TBD | TBD | SSD |

---

## Design Notes

- Nodes are separated by function
- Storage is isolated from compute workloads
- Security environment is fully separated