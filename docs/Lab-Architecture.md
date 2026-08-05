# Lab Architecture

## Project Objective

The objective of this project was to design and administer a virtualized Windows Server environment that simulates common enterprise infrastructure.

The lab includes multiple Windows Server 2022 systems configured to provide centralized identity management, network services, administration, backup, and recovery capabilities.

## Environment Overview

| System | Role | Purpose |
|---|---|---|
| DC1 | Primary Domain Controller | Hosts Active Directory Domain Services, DNS, and DHCP |
| TOR | Additional Domain Controller | Provides domain redundancy and Global Catalog services |
| SVR1 | Member Server | Supports domain-based administration and server services |
| VMware Workstation | Virtualization platform | Hosts and connects the virtual servers |

## Domain Configuration

```text
Domain: adatum.com

DC1
├── Active Directory Domain Services
├── DNS
├── DHCP
└── Primary domain administration

TOR
├── Additional Domain Controller
├── Global Catalog
└── Active Directory replication

SVR1
├── Domain member server
└── Internal server services
