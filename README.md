# Enterprise Active Directory & ServiceNow Lab

## Overview

This project demonstrates the deployment and administration of an enterprise Active Directory environment using **Windows Server 2022 Datacenter: Azure Edition** hosted in **Microsoft Azure**.

The lab simulates real-world IT Support and Help Desk operations by integrating **Active Directory** with **ServiceNow**. Throughout the project, common enterprise administrative tasks such as user provisioning, password resets, account management, Organizational Unit administration, and incident documentation are performed to mirror day-to-day responsibilities of Help Desk Technicians and Junior System Administrators.

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

# Skills Demonstrated

- Azure Virtual Machine Deployment
- Windows Server Administration
- Active Directory Installation & Configuration
- Domain Controller Promotion
- Organizational Unit Administration
- User Account Management
- Security Group Administration
- Password Reset Procedures
- Account Unlock Procedures
- New Employee Onboarding
- ServiceNow Incident Management
- Enterprise Help Desk Documentation

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

# Project Objectives

The primary objectives of this lab are to:

- Deploy a Windows Server 2022 virtual machine in Microsoft Azure.
- Configure an enterprise Active Directory environment.
- Promote the server to a Domain Controller.
- Create and organize Organizational Units.
- Provision and manage Active Directory user accounts.
- Create and manage security groups.
- Simulate common Help Desk scenarios using ServiceNow.
- Document enterprise IT workflows using professional technical documentation.

---

# Future Improvements

Planned enhancements for this lab include:

- Joining Windows 11 client computers to the Active Directory domain.
- Configuring Group Policy Objects (GPOs).
- Creating additional ServiceNow request and incident scenarios.
- Implementing shared folder permissions using security groups.
- Deploying Microsoft Entra ID (Azure AD) integration.
- Configuring Windows Server Update Services (WSUS).
