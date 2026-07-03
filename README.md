# Enterprise Active Directory & ServiceNow Lab

## Overview

This project demonstrates the deployment of an enterprise Windows Server 2022 Active Directory environment hosted in Microsoft Azure. The lab simulates real-world Help Desk scenarios using ServiceNow, including password resets, account unlocks, Organizational Unit management, security groups, and user administration.

---

## Technologies

- Microsoft Azure
- Windows Server 2022 Datacenter: Azure Edition
- Active Directory
- DNS
- DHCP
- IIS
- Group Policy
- ServiceNow

---

## Documentation

The complete walkthrough for each stage of the project can be found below.

| Documentation | Description |
|---------------|-------------|
| [Azure Deployment](docs/01-Azure-Deployment.md) | Creating the Azure Virtual Machine |
| [Installing Active Directory](docs/02-Active-Directory-Installation.md) | Installing AD DS and promoting the Domain Controller |
| [Organizational Units](docs/03-Organizational-Units.md) | Building the company structure |
| [User Management](docs/04-User-Management.md) | Creating and managing Active Directory users |
| [ServiceNow Help Desk Lab](docs/05-ServiceNow-Lab.md) | Password resets and incident management |
| [Security Groups](docs/06-Group-Management.md) | Managing Active Directory Groups |
| [Branch Management](docs/07-Branch-Management.md) | Creating additional branches and moving users |
| [Lessons Learned](docs/08-Lessons-Learned.md) | Skills gained throughout the project |
