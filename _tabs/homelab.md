---
title: Homelab
icon: fas fa-server
order: 5
---

# HomeLab Infrastructure

An overview of my "enterprise-grade" homelab infrastructure with server specifications, capabilities, and architecture.

## Current Infrastructure

My homelab consists of three Proxmox virtualization hosts and a Windows Server 2022 domain controller, providing a robust platform for testing and development.

### Server Fleet

#### Dell PowerEdge R720
- **CPU**: 2× Intel Xeon E5-2450L v2 (20 cores, 40 threads)
- **RAM**: 384 GB
- **Storage**: 24× 600GB 2.5" SAS (14.4 TB total)
- **Hypervisor**: Proxmox VE
- **Role**: Primary virtualization host

#### Dell PowerEdge R630
- **CPU**: 2× Intel Xeon E5-2650L v4 (28 cores, 56 threads)
- **RAM**: 384 GB
- **Storage**: 4× 900GB 2.5" SAS + 6× 600GB 2.5" SAS (7.2 TB total)
- **Hypervisor**: Proxmox VE
- **Role**: Secondary virtualization host

#### HPE ML110
- **CPU**: Intel Xeon Gold 5120 (14 cores, 28 threads)
- **RAM**: 384 GB
- **Storage**: 4× 1TB 3.5" SATA (4 TB total)
- **Hypervisor**: Proxmox VE
- **Role**: Tertiary virtualization host

#### Dell XPS 8700 Workstation
- **CPU**: Intel Core i7-4790 (4 cores, 8 threads, 3.6GHz up to 4.0GHz)
- **RAM**: 16GB DDR3 1600MHz (4x4GB)
- **Storage**: 2TB 7200RPM HDD + 32GB mSATA SSD (2.03 TB total)
- **Graphics**: NVIDIA GeForce GTX 750Ti 2GB DDR5
- **OS**: Windows Server 2022
- **Role**: Active Directory / Domain Controller

## Infrastructure Specifications

| Resource | Capacity |
|----------|----------|
| CPU Cores | 62 physical cores |
| CPU Threads | 124 logical processors |
| Total RAM | 1,152 GB |
| Total Storage | 27.63 TB raw |
| Virtualization | Proxmox VE (3 hosts) |
| Network Services | Active Directory, DNS |

## Current Projects

I'm working on several infrastructure projects in my homelab environment:

- Hyper-converged storage with Ceph
- Kubernetes cluster for container orchestration
- CI/CD pipeline with GitLab
- Network segmentation with VLANs
- Centralized logging and monitoring
- High availability service deployment

## Future Plans

I'm planning to expand my homelab with the following:

- 10GbE networking between hosts
- Additional storage nodes
- Hardware security modules
- Redundant power with UPS integration
- Edge computing nodes

## Blog Posts

Check back for detailed write-ups on my homelab journey, including:

- Setting up Proxmox clustering
- Configuring Active Directory integration
- Storage optimization techniques
- VM template management
- Backup and disaster recovery strategies
- Power consumption optimization