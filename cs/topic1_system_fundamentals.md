# Topic 1: System Fundamentals

> SL + HL | Core Topic

## Key Concepts

### 1.1 Systems in Organizations

#### Planning and System Installation
- System lifecycle: planning → analysis → design → implementation → maintenance
- **Change management**: how organizations prepare people and processes for new systems
  - Involves engaging stakeholders, providing training, and producing documentation
- Implementation strategies:
  - **Parallel**: old and new systems run simultaneously
  - **Phased**: gradual rollout by module or department
  - **Direct changeover**: immediate switch (highest risk)
  - **Pilot**: tested in one area before full deployment

#### User Focus
- **Usability**: how easily and efficiently users can accomplish tasks
- **Accessibility**: designing so that people with disabilities can use the system effectively
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
- **Disaster recovery plan**: a documented set of procedures that guides restoring operations after a serious failure or catastrophe
- Data integrity and validation

### 1.4 Software Deployment

- **Software release types**: alpha, beta, release candidate, production
- **Licensing**: proprietary, open source, freeware, shareware
- **Software as a Service (SaaS)** vs. on-premise installation
- Automatic updates and patch management

## Key Terminology

| Term | Definition |
|------|-----------|
| **Stakeholder** | Anyone who has an interest in or is affected by a system's operation |
| **Parallel implementation** | A transition approach where both old and new systems operate at the same time |
| **Data flow diagram** | A diagram that shows the movement and transformation of data through a system |
| **Redundancy** | Having duplicate components or data so that a failure in one does not bring the system down |
| **SaaS** | A model where software is hosted remotely and accessed over the internet |
| **UAT** | User acceptance testing; the stage where real end-users confirm the system meets their needs |
| **RAID** | Redundant Array of Independent Disks; uses multiple drives together for data protection or performance |

## Common Misconceptions

1. **"Direct changeover is the safest implementation method"** — It is actually the riskiest approach; parallel running gives a safety net but costs more.
2. **"Backups prevent data loss"** — Backups make recovery possible after data is lost; they do not stop the loss from occurring in the first place.
3. **"System design is only about technology"** — People, workflows, and organizational context shape system design just as much as technical choices do.
4. **"Open source means free and unsupported"** — Open source describes how source code is licensed and shared; many open-source projects have paid professional support options.

## Comparison with AP CS

- AP CS A does not cover system fundamentals or organizational aspects
- AP CS Principles covers some system concepts (internet, data, impact) but with less depth on implementation strategies
- IB CS uniquely covers change management and system lifecycle from an organizational perspective
