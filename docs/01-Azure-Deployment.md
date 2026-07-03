# Azure Virtual Machine Deployment

## Objective

The goal of this section is to deploy a Windows Server 2022 Datacenter: Azure Edition virtual machine in Microsoft Azure. This virtual machine will serve as the Domain Controller for the Active Directory environment built throughout this project.

---

## Lab Environment

| Component | Configuration |
|-----------|---------------|
| Cloud Platform | Microsoft Azure |
| Operating System | Windows Server 2022 Datacenter: Azure Edition |
| Virtual Machine Purpose | Domain Controller |
| Remote Access | Azure Bastion |

---

# Step 1 - Deploying the Virtual Machine

### Overview

A Windows Server 2022 Datacenter: Azure Edition virtual machine was created through the Microsoft Azure Portal. This virtual machine will later host Active Directory Domain Services, DNS, DHCP, and other Windows Server roles required for the lab.

### Procedure

1. Signed into the Microsoft Azure Portal.
2. Selected **Create a Virtual Machine**.
3. Chose **Windows Server 2022 Datacenter: Azure Edition** as the operating system.
4. Selected the appropriate VM size.
5. Configured administrator credentials.
6. Deployed the virtual machine.

### Result

The Windows Server virtual machine deployed successfully and became available for management through Azure.

### Screenshot

*<img width="1690" height="874" alt="Azure VM Lab Creation" src="https://github.com/user-attachments/assets/38cacb03-883c-4d93-8414-d0afb5ce3a95" /><img width="1696" height="879" alt="Azure VM Static Networking Configuration" src="https://github.com/user-attachments/assets/7611939b-f303-4a54-970c-0bbcf19ac04b" />


---

# Step 2 - Configuring a Static Private IP Address

### Overview

A static private IP address was assigned to the virtual machine to ensure the Domain Controller always maintains the same internal network address.

### Why This Matters

Domain Controllers should always use a static IP address because Active Directory and DNS rely on consistent network communication.

### Procedure

1. Opened the Networking settings.
2. Selected the Network Interface.
3. Changed the Private IP Assignment from **Dynamic** to **Static**.
4. Saved the configuration.

### Result

The virtual machine now maintains a permanent private IP address.

### Screenshot

<img width="1696" height="879" alt="Azure VM Static Networking Configuration" src="https://github.com/user-attachments/assets/56e62f4c-b2d0-42d1-a0c8-456c15d1f09e" />


---

# Step 3 - Connecting with Azure Bastion

### Overview

Azure Bastion was used to securely connect to the virtual machine without exposing Remote Desktop Protocol (RDP) to the public internet.

### Why Azure Bastion

Using Azure Bastion improves security by allowing browser-based access over HTTPS while eliminating the need to open inbound RDP ports.

### Procedure

1. Opened the virtual machine in Azure.
2. Selected **Connect**.
3. Chose **Bastion**.
4. Logged into the server using administrator credentials.

### Result

A secure remote connection to the Windows Server virtual machine was successfully established.

### Screenshot

*(Insert Screenshot 3 Here)*
