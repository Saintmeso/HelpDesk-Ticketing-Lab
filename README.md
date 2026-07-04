# Enterprise Active Directory & ServiceNow Lab

## Business Problem

Organizations rely on centralized identity management and ticketing systems to efficiently manage employee accounts and IT support requests. Without a centralized solution, administrators must manually manage user accounts, permissions, and troubleshooting tasks, increasing the likelihood of security risks, inconsistent configurations, and longer resolution times.

This project simulates a small enterprise environment by deploying a Windows Server 2022 Domain Controller in Microsoft Azure and integrating Active Directory with ServiceNow. The environment demonstrates how IT administrators can centrally manage users, organizational structure, and common Help Desk requests such as password resets, account unlocks, and new employee onboarding.

---

# Project Architecture

```text
                         Microsoft Azure
                                │
                    Windows Server 2022 VM
                                │
        ┌───────────────────────┴────────────────────────┐
        │                                                │
 Active Directory Domain Services                  Azure Bastion
        │
        ├── DNS
        ├── DHCP
        ├── Group Policy Management
        ├── Organizational Units
        ├── Users
        └── Security Groups
                │
                ▼
      ServiceNow Developer Instance
                │
        ├── Password Reset Requests
        ├── Account Unlock Requests
        └── New Employee Onboarding
```

---

# Key Design Decisions

## 1. Secure Administrative Access with Azure Bastion

Instead of exposing Remote Desktop (RDP) directly to the internet, Azure Bastion was used to securely manage the Windows Server through the Azure Portal. This reduces the attack surface by eliminating the need for a public RDP endpoint while still allowing remote administration.

---

## 2. Organizational Unit Structure

Rather than placing every object in the default Active Directory containers, Organizational Units were created to separate users, computers, and groups. This mirrors how enterprise environments organize resources and provides a scalable structure for future Group Policy deployment and administrative delegation.

---

## 3. Integrating Active Directory with ServiceNow

Instead of demonstrating Active Directory administration in isolation, ServiceNow was incorporated to simulate realistic Help Desk workflows. Common support tasks—including password resets, account unlocks, and new employee onboarding—were documented from ticket creation through resolution, reflecting day-to-day enterprise IT operations.

---

# Technologies

- Microsoft Azure
- Windows Server 2022 Datacenter: Azure Edition
- Azure Bastion
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers (ADUC)
- DNS Server
- DHCP Server
- Internet Information Services (IIS)
- Group Policy Management
- ServiceNow Developer Instance

---

# Documentation

The following documentation provides a complete walkthrough of the lab environment and the administrative tasks performed throughout the project.

| Documentation | Description |
|---------------|-------------|
| [Azure Deployment](docs/01-Azure-Deployment.md) | Deploying a Windows Server 2022 virtual machine in Microsoft Azure and configuring networking. |
| [Active Directory Installation](docs/02-Active-Directory-Installation.md) | Installing Windows Server roles and promoting the server to a Domain Controller. |
| [Organizational Unit Management](docs/03-Organizational-Units.md) | Creating Organizational Units to organize the Active Directory environment. |
| [User & Group Administration](docs/04-User-and-Group-Administration.md) | Creating users, managing user accounts, and administering security groups. |
| [ServiceNow Help Desk Lab](docs/05-ServiceNow-Help-Desk-Lab.md) | Simulating a Help Desk password reset and account unlock workflow using ServiceNow and Active Directory. |
| [New Employee Onboarding](docs/06-New-Employee-Onboarding.md) | Provisioning a new employee account through ServiceNow and Active Directory. |
| [Lessons Learned](docs/07-Lessons-Learned.md) | Summary of skills developed, project outcomes, and future improvements. |

---

# Technologies & Skills Demonstrated

### Infrastructure

- Microsoft Azure
- Windows Server 2022 Datacenter: Azure Edition
- Azure Bastion

### Identity & Directory Services

- Active Directory Domain Services
- DNS
- DHCP
- Organizational Units
- User & Group Management

### IT Operations

- ServiceNow Incident Management
- Password Reset Procedures
- Account Unlock Procedures
- New Employee Onboarding
- Enterprise Help Desk Documentation

---

# Future Improvements

- Deploy a Windows 11 client and join it to the Active Directory domain.
- Configure Group Policy Objects (GPOs) for centralized workstation management.
- Expand the ServiceNow environment with additional enterprise support scenarios.
- Implement shared folder permissions using Active Directory security groups.
- Integrate Microsoft Entra ID for hybrid identity management.
- Configure Windows Server Update Services (WSUS).
