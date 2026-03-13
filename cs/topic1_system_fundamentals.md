# Topic 1: System Fundamentals

> SL + HL | Core Topic

## Key Concepts

### 1.1 Systems in Organizations

#### Planning and System Installation
- System lifecycle: planning → analysis → design → implementation → maintenance
- **Change management**: preparing organizations for new systems
  - Stakeholder involvement, training, documentation
- Implementation strategies:
  - **Parallel**: old and new systems run simultaneously
  - **Phased**: gradual rollout by module or department
  - **Direct changeover**: immediate switch (highest risk)
  - **Pilot**: tested in one area before full deployment

#### User Focus
- **Usability**: ease of use, learnability, efficiency
- **Accessibility**: designing for users with disabilities
- End-user training and documentation
- User acceptance testing (UAT)

### 1.2 System Design Basics

#### Components of a Computer System
- **Hardware**: physical components (CPU, memory, storage, I/O devices)
- **Software**: programs and operating systems
  - System software vs. application software
- **Peripherals**: input devices, output devices, storage devices
- **Network components**: routers, switches, cables, wireless access points

#### System Design and Analysis
- Identifying stakeholders and their requirements
- **Data flow diagrams (DFDs)**: visual representation of data movement
- **System flowcharts**: showing processes and decisions
- Feasibility study: technical, economic, legal, operational, schedule (TELOS)

### 1.3 System Backup and Data Loss

- Causes of data loss: hardware failure, human error, malware, natural disasters
- **Backup strategies**:
  - Full backup, incremental backup, differential backup
  - On-site vs. off-site vs. cloud backup
- **Redundancy**: RAID configurations, failover systems
- **Disaster recovery plan**: procedures for restoring operations after catastrophic failure
- Data integrity and validation

### 1.4 Software Deployment

- **Software release types**: alpha, beta, release candidate, production
- **Licensing**: proprietary, open source, freeware, shareware
- **Software as a Service (SaaS)** vs. on-premise installation
- Automatic updates and patch management

## Key Terminology

| Term | Definition |
|------|-----------|
| **Stakeholder** | Any person affected by or having interest in a system |
| **Parallel implementation** | Running old and new systems simultaneously during transition |
| **Data flow diagram** | Visual model showing how data moves through a system |
| **Redundancy** | Duplication of critical components for fault tolerance |
| **SaaS** | Software delivered over the internet as a service |
| **UAT** | User acceptance testing; end-users validate the system meets requirements |
| **RAID** | Redundant Array of Independent Disks; provides data redundancy |

## Common Misconceptions

1. **"Direct changeover is the safest implementation method"** -- It is the riskiest; parallel running is safest but most expensive.
2. **"Backups prevent data loss"** -- Backups allow recovery after data loss; they do not prevent the initial loss.
3. **"System design is only about technology"** -- Human factors, organizational change, and stakeholder needs are equally important.
4. **"Open source means free and unsupported"** -- Open source refers to the license; many open-source projects have professional support.

## Comparison with AP CS

- AP CS A does not cover system fundamentals or organizational aspects
- AP CS Principles covers some system concepts (internet, data, impact) but with less depth on implementation strategies
- IB CS uniquely covers change management and system lifecycle from an organizational perspective
