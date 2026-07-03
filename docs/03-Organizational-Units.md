# Organizational Unit (OU) Management

## Objective

The goal of this section is to organize the Active Directory environment by creating Organizational Units (OUs). Organizational Units allow administrators to logically separate users, computers, and security groups, making Active Directory easier to manage and preparing the environment for future Group Policy deployment.

---

## Lab Environment

| Component | Configuration |
|-----------|---------------|
| Operating System | Windows Server 2022 Datacenter: Azure Edition |
| Management Tool | Active Directory Users and Computers (ADUC) |
| Domain | *Your Domain Name* |
| Administrative Tool | Server Manager / ADUC |

---

# Step 1 - Opening Active Directory Users and Computers

### Overview

After successfully promoting the server to a Domain Controller, Active Directory Users and Computers (ADUC) was opened to begin organizing the Active Directory environment.

ADUC is the primary administrative tool used by IT professionals to manage users, computers, groups, and Organizational Units within a Windows domain.

### Procedure

1. Opened the Windows Search bar.
2. Searched for **Active Directory Users and Computers**.
3. Launched the management console.

### Result

The Active Directory management console opened successfully and displayed the domain structure.

### Screenshot

*<img width="752" height="530" alt="Azure VM AD Dashboard" src="https://github.com/user-attachments/assets/842f93e4-0434-400d-b67c-5397d9c1be54" />

---

# Step 2 - Creating the First Organizational Unit

### Overview

The first Organizational Unit (OU) was created to represent the organization's primary branch.

Organizational Units provide a logical structure within Active Directory, allowing administrators to organize objects based on departments, locations, or business units.

### Why Use Organizational Units?

Organizational Units make Active Directory easier to manage by allowing administrators to:

- Organize users and computers
- Apply Group Policy to specific departments
- Delegate administrative permissions
- Keep the directory organized as the environment grows

### Procedure

1. Right-clicked the domain.
2. Selected **New** → **Organizational Unit**.
3. Named the Organizational Unit **Branch 1**.
4. Selected **OK**.

### Result

A new Organizational Unit named **Branch 1** was successfully created.

### Screenshot

<img width="752" height="528" alt="Azure VM AD Organization Unit created (branch 1)" src="https://github.com/user-attachments/assets/f65a52d0-653a-44bf-b261-a4f12c7700fe" />

---

# Step 3 - Creating Department Organizational Units

### Overview

To further organize the Active Directory environment, three additional Organizational Units were created inside **Branch 1**.

These Organizational Units separate users, computers, and security groups into their own administrative containers.

### Organizational Units Created

**Users**

Stores employee user accounts.

**Computers**

Stores computers that will eventually join the domain.

**Groups**

Stores security groups used for assigning permissions and managing access.

### Procedure

1. Opened the **Branch 1** Organizational Unit.
2. Right-clicked **Branch 1**.
3. Selected **New** → **Organizational Unit**.
4. Repeated the process to create:

- Users
- Computers
- Groups

### Result

The Active Directory environment now contains a structured hierarchy for managing organizational resources.

### Screenshot

<img width="752" height="527" alt="Azure VM AD Branch 1 Sub OU&#39;s" src="https://github.com/user-attachments/assets/a53a8a95-f546-4dec-8ae4-e70a510a07ee" />

---

# Organizational Structure

The Organizational Unit hierarchy now resembles the following structure:

```text
YourDomain.local
│
└── Branch 1
     ├── Users
     ├── Computers
     └── Groups
```

This structure provides a scalable foundation for future expansion as additional branches, departments, and resources are added.

---

# Summary

In this section, the Active Directory environment was organized by creating Organizational Units.

The following tasks were completed:

- Opened Active Directory Users and Computers
- Created the Branch 1 Organizational Unit
- Created separate Organizational Units for Users, Computers, and Groups
- Established a logical directory structure for future user, computer, and security group management

The Active Directory environment is now organized and prepared for user account creation, group administration, and future Group Policy implementation.
