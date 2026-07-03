# Active Directory Installation & Domain Controller Configuration

## Objective

The goal of this section is to install the Windows Server roles required to build an enterprise Active Directory environment and promote the Windows Server 2022 virtual machine to a Domain Controller.

By the end of this section, the server will be configured to provide centralized authentication and directory services for the organization.

---

## Lab Environment

| Component | Configuration |
|-----------|---------------|
| Operating System | Windows Server 2022 Datacenter: Azure Edition |
| Server Manager | Windows Server Manager |
| Active Directory | Active Directory Domain Services (AD DS) |
| DNS | Installed |
| DHCP | Installed |
| IIS | Installed |
| Print Services | Installed |
| Group Policy | Installed |

---

# Step 1 - Verifying Active Directory is Not Installed

### Overview

After connecting to the Windows Server virtual machine, Server Manager was opened to verify that Active Directory Domain Services had not yet been installed.

This confirms that the server is in its default state before beginning the installation process.

### Procedure

1. Opened **Server Manager**.
2. Selected **Manage**.
3. Chose **Add Roles and Features**.

### Result

The Add Roles and Features Wizard opened, allowing Windows Server roles and features to be installed.

### Screenshot

<img width="1685" height="741" alt="Azure VM AD Not downloaded" src="https://github.com/user-attachments/assets/08d3fdb4-d3bc-4b61-8bd3-acedc1a7730c" />

---

# Step 2 - Installing Required Windows Server Roles

### Overview

Several Windows Server roles were installed to simulate a realistic enterprise network environment.

Each server role provides a specific service commonly used within business networks.

### Roles Installed

**Active Directory Domain Services (AD DS)**

Provides centralized authentication, user management, and directory services throughout the network.

**DNS Server**

Resolves computer and domain names into IP addresses, allowing devices to communicate across the network.

**DHCP Server**

Automatically assigns IP addresses and network configuration information to client devices.

**Print and Document Services**

Provides centralized management of printers and document services within an organization.

**Web Server (IIS)**

Hosts websites and web applications while allowing the server to function as a web server.

### Procedure

1. Opened **Add Roles and Features Wizard**.
2. Selected **Role-based or feature-based installation**.
3. Chose the local server.
4. Selected all required Windows Server roles.
5. Continued through the installation wizard.

### Result

Windows Server began installing all selected server roles.

### Screenshot

*(Insert Screenshot 5 Here)*

---

# Step 3 - Installing Group Policy Management

### Overview

While installing Active Directory Domain Services, Windows prompted the installation of additional management features.

One of the most important features selected was **Group Policy Management**.

### Why Group Policy Management?

Group Policy allows administrators to centrally manage computers and users across an Active Directory environment.

Common uses include:

- Password Policies
- Desktop Restrictions
- Software Deployment
- Security Policies
- Windows Update Configuration
- User Configuration

Group Policy is one of the core administrative tools used in enterprise environments.

### Procedure

1. Selected **Add Features** when prompted.
2. Verified that **Group Policy Management** was selected.
3. Continued through the installation.

### Result

Group Policy Management was installed alongside Active Directory Domain Services.

### Screenshot

*(Insert Screenshot 6 Here)*

---

# Step 4 - Verifying Successful Installation

### Overview

After the installation completed successfully, Server Manager displayed the newly installed server roles.

This confirmed that Active Directory Domain Services and the remaining services had been installed correctly.

### Procedure

1. Waited for the installation to finish.
2. Reviewed the Server Manager Dashboard.

### Result

The server roles appeared successfully within Server Manager and were ready for configuration.

### Screenshot

*(Insert Screenshot 7 Here)*

---

# Step 5 - Promoting the Server to a Domain Controller

### Overview

Installing Active Directory Domain Services alone does not create a Domain Controller.

An additional configuration step is required to promote the server into an Active Directory Domain Controller.

### Why Promote to a Domain Controller?

A Domain Controller is responsible for:

- Authenticating users
- Managing Active Directory
- Applying Group Policies
- Managing security
- Storing directory information

Without promoting the server, Active Directory cannot be used.

### Procedure

1. Selected the notification flag in Server Manager.
2. Chose **Promote this server to a domain controller**.

### Result

The Active Directory Domain Services Configuration Wizard opened.

### Screenshot

*(Insert Screenshot 8 Here)*

---

# Step 6 - Creating a New Active Directory Forest

### Overview

Since this environment was being built from scratch, a new Active Directory Forest was created.

The forest represents the highest level of the Active Directory hierarchy.

### Why Create a New Forest?

Creating a new forest establishes:

- A new Active Directory environment
- A new domain
- A centralized authentication system
- The root of the organization's directory structure

A root domain name was assigned during this process.

### Procedure

1. Selected **Add a new forest**.
2. Entered the desired root domain name.
3. Continued through the configuration wizard.

### Result

The Active Directory forest configuration was successfully created.

### Screenshot

*(Insert Screenshot 9 Here)*

---

# Step 7 - Completing Prerequisite Checks

### Overview

Before promoting the server, Windows automatically performed several prerequisite validation checks.

These checks ensure the server is properly configured before becoming a Domain Controller.

### Procedure

1. Reviewed prerequisite warnings.
2. Confirmed all required checks passed.
3. Selected **Install**.

### Result

Windows promoted the server to a Domain Controller.

The server automatically restarted to complete the installation.

### Screenshot

*(Insert Screenshot 10 Here)*

---

# Step 8 - Accessing Active Directory Users and Computers

### Overview

After the server rebooted, Active Directory Domain Services became fully operational.

The **Active Directory Users and Computers (ADUC)** management console was opened to begin administering the new Active Directory environment.

### Why Use ADUC?

Active Directory Users and Computers is the primary administrative tool used to manage:

- Users
- Computers
- Security Groups
- Organizational Units
- Password Resets
- Account Unlocks
- User Properties

This console is one of the most frequently used tools by Help Desk Technicians and System Administrators.

### Procedure

1. Opened the Windows Search bar.
2. Launched **Active Directory Users and Computers**.

### Result

The Active Directory environment was ready for administration.

### Screenshot

*(Insert Screenshot 11 Here)*

---

# Summary

In this section, the Windows Server 2022 virtual machine was successfully transformed into a fully functional Active Directory Domain Controller.

The following tasks were completed:

- Installed Active Directory Domain Services (AD DS)
- Installed DNS Server
- Installed DHCP Server
- Installed Print and Document Services
- Installed IIS Web Server
- Installed Group Policy Management
- Promoted the server to a Domain Controller
- Created a new Active Directory Forest
- Completed prerequisite validation
- Verified Active Directory functionality using Active Directory Users and Computers (ADUC)

The Active Directory environment is now fully operational and ready for Organizational Unit creation, user management, and enterprise administration tasks.
