# User & Group Administration

## Objective

The goal of this section is to manage user accounts and security groups within Active Directory. This includes creating employee accounts, organizing users, assigning group memberships, and maintaining user information.

These tasks represent common responsibilities performed by Help Desk Technicians and System Administrators in enterprise environments.

---

## Lab Environment

| Component | Configuration |
|-----------|---------------|
| Operating System | Windows Server 2022 Datacenter: Azure Edition |
| Management Tool | Active Directory Users and Computers (ADUC) |
| Organizational Unit | Branch 1 |

---

# Step 1 - Creating the First User Account

### Overview

The first employee account was created inside the **Users** Organizational Unit.

Each user account contains identifying information that allows employees to authenticate to the domain and access organizational resources.

### Procedure

1. Opened **Branch 1**.
2. Opened the **Users** Organizational Unit.
3. Right-clicked inside the OU.
4. Selected **New** → **User**.
5. Entered the employee's:
   - First Name
   - Last Name
   - Username (User Logon Name)
6. Assigned an initial password.
7. Completed the user creation wizard.

### Result

A new Active Directory user account was successfully created.

### Screenshot

<img width="437" height="379" alt="Azure VM AD USER CREATION" src="https://github.com/user-attachments/assets/3ee22018-9ad3-4d3b-8a7b-9a44cbed1a03" />
<img width="437" height="377" alt="Azure VM AD USER CREATION PASSWORD" src="https://github.com/user-attachments/assets/8384b006-fb8e-4a88-b9d0-7eb7e93a11f9" />

---

# Step 2 - Verifying User Creation

### Overview

After completing the user creation wizard, the account appeared within the Users Organizational Unit.

Verifying the account ensures that Active Directory successfully created the new object.

### Procedure

1. Refreshed the Users Organizational Unit.
2. Located the newly created employee account.

### Result

The user account appeared successfully inside Active Directory.

### Screenshot

<img width="756" height="525" alt="Azure VM AD USER CREATION CONFIRMATION" src="https://github.com/user-attachments/assets/f5e12456-a3a8-4f66-98af-89f8f94f1af5" />

---

# Step 3 - Creating Additional Employee Accounts

### Overview

To simulate a realistic business environment, multiple employee accounts were created.

Creating multiple users allows Active Directory administration tasks to be performed in a more realistic enterprise environment.

### Procedure

The same user creation process was repeated to create several employee accounts.

Each account was assigned:

- First Name
- Last Name
- Username
- Password

### Result

The Active Directory environment now contains multiple employee accounts that can be used throughout the remainder of the lab.

### Screenshot

<img width="756" height="524" alt="image" src="https://github.com/user-attachments/assets/f0daff94-d43a-47d9-a807-78e35f990bb5" />


---

# Step 4 - Creating the IT Workers Security Group

### Overview

A security group named **IT Workers** was created to represent employees responsible for IT administration.

Security groups simplify permission management by assigning permissions to groups instead of individual users.

### Why Use Security Groups?

Security groups allow administrators to:

- Assign permissions once
- Control access efficiently
- Simplify administration
- Reduce configuration errors

### Procedure

1. Opened the **Groups** Organizational Unit.
2. Right-clicked inside the OU.
3. Selected **New** → **Group**.
4. Named the group **IT Workers**.
5. Completed the wizard.

### Result

The IT Workers security group was successfully created.

### Screenshot

<img width="756" height="497" alt="Azure VM AD Group Creation IT workers" src="https://github.com/user-attachments/assets/dd56e7bf-85e4-4299-9135-bebfbba48bd9" />

---

# Step 5 - Adding a User to the IT Workers Group

### Overview

The user **Noah Hayes** was added to the IT Workers security group.

Adding users to security groups allows administrators to assign permissions based on job roles rather than configuring each user individually.

### Procedure

1. Opened the **IT Workers** group.
2. Selected **Members**.
3. Added **Noah Hayes**.
4. Applied the changes.

### Result

Noah Hayes became a member of the IT Workers security group.

### Screenshot

<img width="401" height="452" alt="Azure VM AD IT Worker User add Noah Hayes" src="https://github.com/user-attachments/assets/f2d06dd0-cbcf-4708-84c3-55a53505d9bc" />

---

# Step 6 - Creating a New User Using Copy

### Overview

Instead of creating another employee account from scratch, an existing user account was copied.

Copying users saves time because many account settings and group memberships are automatically inherited.

The existing user **Noah Hayes** was copied to create a new employee named **Adam Smith**.

### Why Copy User Accounts?

Copying users helps administrators:

- Speed up onboarding
- Maintain consistent permissions
- Reduce manual configuration
- Prevent configuration mistakes

### Procedure

1. Right-clicked **Noah Hayes**.
2. Selected **Copy**.
3. Entered the new employee information.
4. Assigned a password.
5. Completed the wizard.

### Result

A new user account named Adam Smith was created.

### Screenshot

<img width="752" height="496" alt="Azure VM AD It worker Copy Adam Smith" src="https://github.com/user-attachments/assets/dd21832f-40e7-4080-8c7e-47f10ac972ef" />

---

# Step 7 - Verifying Group Membership Inheritance

### Overview

Because Adam Smith was created using the Copy feature, he automatically inherited membership within the **IT Workers** security group.

This demonstrates one of the advantages of copying existing user accounts.

### Procedure

1. Opened Adam Smith's properties.
2. Selected the **Member Of** tab.

### Result

Adam Smith was automatically listed as a member of the IT Workers security group.

### Screenshot

<img width="408" height="537" alt="Pic of adam smith confirming he is in IT workers" src="https://github.com/user-attachments/assets/65c8b7b5-254f-4449-ae8c-962782e18cd3" />

---

# Step 8 - Updating User Properties

### Overview

Additional information was added to each user account to better simulate a real enterprise environment.

Updating user properties improves administration, reporting, and identity management.

### Information Added

- Job Title
- Department
- Organization
- Description

### Procedure

1. Opened the user's Properties.
2. Updated the appropriate profile information.
3. Saved the changes.

### Result

Each employee account now contains organizational information commonly maintained in Active Directory.

### Screenshot

<img width="754" height="521" alt="Added Description of users" src="https://github.com/user-attachments/assets/9de1eb64-eb80-4681-88a3-4b04c5c62ccb" />
<img width="410" height="541" alt="Examples of Organization info for users" src="https://github.com/user-attachments/assets/c86f8abc-aaba-40f5-8962-f6b70fe67b8e" />
<img width="408" height="538" alt="Examples 2 of Organization info for users" src="https://github.com/user-attachments/assets/212aef9e-277e-49a9-a2e3-0ee8d3e422c1" />

---

# Summary

In this section, Active Directory user and security group administration tasks were completed.

The following tasks were successfully performed:

- Created employee user accounts
- Verified account creation
- Created multiple users
- Created the IT Workers security group
- Added users to a security group
- Created a new employee using the Copy feature
- Verified inherited group membership
- Updated employee profile information

The Active Directory environment now contains a realistic organizational structure with users and security groups that can be used throughout the Help Desk scenarios.
