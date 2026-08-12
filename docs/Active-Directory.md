# Active Directory Administration

## Overview

This section documents the Active Directory administration work completed within my Windows Server enterprise lab.

The environment was designed to provide hands-on experience with centralized identity management, domain controllers, organizational units, security groups, delegated administration, service accounts, Active Directory replication, Global Catalog services, and PowerShell-based administration.

## Environment

| Component          | Role                         |
| ------------------ | ---------------------------- |
| **Domain**         | `adatum.com`                 |
| **DC1**            | Primary Domain Controller    |
| **TOR**            | Additional Domain Controller |
| **SVR1**           | Domain-joined Member Server  |
| **Platform**       | Windows Server 2022          |
| **Virtualization** | VMware Workstation           |

## Active Directory Domain Services

Active Directory Domain Services (AD DS) was used to provide centralized authentication and administration for the Windows Server lab.

The environment included multiple domain controllers to practice administration in a multi-server domain rather than relying on a single Windows Server instance.

### Skills Practiced

* Active Directory Domain Services
* Domain Controller administration
* Organizational Units
* User and Group management
* Security Groups
* Delegated Administration
* Service Accounts
* Global Catalog
* FSMO role administration
* Active Directory PowerShell
* Active Directory maintenance

---

## Domain Controllers

The lab contained two domain controllers:

### DC1

DC1 operated as the primary domain controller for the lab and provided core Active Directory services.

### TOR

TOR was configured as an additional domain controller.

Working with multiple domain controllers provided experience with:

* Domain Controller promotion
* Active Directory replication
* Global Catalog configuration
* Active Directory Sites and Services
* FSMO role administration

---

## Global Catalog

Global Catalog functionality was configured and verified on the TOR domain controller using **Active Directory Sites and Services**.

This exercise provided hands-on experience working with domain controller properties and understanding the role of the Global Catalog within an Active Directory environment.

---

## FSMO Role Administration

The lab included transferring the **RID Master** role to the TOR domain controller.

The successful transfer was verified through Active Directory administration tools and PowerShell.

This provided practical exposure to Flexible Single Master Operations (FSMO) roles and domain controller administration.

---

## Organizational Units and Groups

Organizational Units were used to organize Active Directory objects and support administrative separation.

The lab included creation and administration of security groups, including an **ITAdmins** group within the IT Organizational Unit.

### Tasks Performed

* Created Organizational Units
* Created security groups
* Added members to groups
* Reviewed group properties
* Organized Active Directory objects
* Applied delegated administrative permissions

---

## Delegation of Control

The **Delegation of Control Wizard** was used to assign administrative responsibilities to selected users or groups without granting unrestricted domain-level privileges.

This demonstrated the principle of delegating only the permissions required to perform specific administrative tasks.

---

## Service Accounts

A dedicated **Service Accounts** Organizational Unit was created to separate service identities from standard user accounts.

Service accounts were configured and used with Windows services during the lab.

This provided practical experience with:

* Service account creation
* Organizational separation
* Windows service configuration
* Account permissions
* Service identity management

---

## PowerShell Administration

PowerShell was used to perform and verify Active Directory administrative tasks.

Working with Active Directory through PowerShell demonstrated how repetitive administrative operations can be performed more efficiently than relying exclusively on graphical management consoles.

PowerShell activities are documented separately in:

`PowerShell.md`

---

## Screenshots

Screenshots demonstrating the configuration will be added below.

### Domain Controllers

`Screenshot coming soon`

### Global Catalog

`Screenshot coming soon`

### Security Groups

`Screenshot coming soon`

### Delegation of Control

`Screenshot coming soon`

### Service Accounts

`Screenshot coming soon`

### PowerShell Administration

`Screenshot coming soon`

---

## Key Takeaways

This lab strengthened my understanding of how Active Directory is administered in a multi-server Windows environment.

The most valuable areas of practical experience included:

* Managing multiple domain controllers
* Organizing directory objects using Organizational Units
* Managing users and security groups
* Delegating administrative permissions
* Working with service accounts
* Configuring Global Catalog functionality
* Managing FSMO roles
* Using PowerShell for Active Directory administration

The project also reinforced the importance of structured documentation, controlled administrative permissions, and repeatable troubleshooting procedures in Windows Server environments.

---

[← Back to Main README](../README.md)

