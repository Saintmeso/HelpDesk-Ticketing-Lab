# New Employee Onboarding

## Objective

The goal of this section is to simulate the onboarding process for a new employee by fulfilling an account creation request through ServiceNow and provisioning the employee's Active Directory account.

This workflow demonstrates a common responsibility performed by Help Desk Technicians and System Administrators when preparing a new employee for their first day.

---

## Lab Environment

| Component | Configuration |
|-----------|---------------|
| Cloud Platform | Microsoft Azure |
| Operating System | Windows Server 2022 Datacenter: Azure Edition |
| Directory Service | Active Directory Domain Services |
| Management Tool | Active Directory Users and Computers (ADUC) |
| Ticketing Platform | ServiceNow Developer Instance |

---

# Scenario

**Employee Name:** Emma Wilson

**Department:** Finance

**Job Title:** Financial Analyst

**Organization:** Obeta

**Request:** Provision a new Active Directory account for a newly hired employee.

---

# Step 1 - Creating the ServiceNow Request

### Overview

A ServiceNow request was created to simulate a new employee onboarding request submitted by a hiring manager.

The request included the employee's department, job title, and organization so the account could be configured correctly.

### Procedure

1. Logged into ServiceNow.
2. Created a new request.
3. Entered the employee information.
4. Documented the onboarding requirements.
5. Submitted the request.

### Result

The onboarding request was successfully created and assigned for processing.

### Screenshot

<img width="960" height="867" alt="ServiceNow Emma Wilson Ticket creation" src="https://github.com/user-attachments/assets/42d72314-211b-4bda-bf3a-6c2792ac07c1" />

---

# Step 2 - Creating the Active Directory Account

### Overview

A new Active Directory user account was created for Emma Wilson using Active Directory Users and Computers.

The account was configured with the employee's name, username, and an initial password.

### Procedure

1. Opened Active Directory Users and Computers.
2. Navigated to the Users Organizational Unit.
3. Created a new user account.
4. Assigned a temporary password.
5. Enabled **User must change password at next logon**.
6. Completed the account creation wizard.

### Result

The employee account was successfully created.

### Screenshot

<img width="438" height="377" alt="ServiceNow Emma Wilson Account creation AD" src="https://github.com/user-attachments/assets/6744f7d6-9442-4b12-97f0-ff08927c3ea9" />
<img width="437" height="377" alt="ServiceNow Emma Wilson password creation" src="https://github.com/user-attachments/assets/e1d721cc-c2ba-4cf7-8c45-7e239e540e2e" />

---

# Step 3 - Configuring Employee Information

### Overview

After creating the account, additional organizational information was configured to accurately represent the employee's role within the company.

### Information Configured

- Job Title
- Department
- Organization

Maintaining accurate user properties helps administrators manage users and improves directory organization.

### Procedure

1. Opened the user's Properties.
2. Updated the Organization tab.
3. Saved the changes.

### Result

The employee profile now contains the appropriate organizational information.

### Screenshot

<img width="411" height="536" alt="ServiceNow Emma Wilson Org provisioning" src="https://github.com/user-attachments/assets/04aa6065-e2ea-41be-a451-5064f1134a47" />

---

# Step 4 - Verifying Account Creation

### Overview

After completing the configuration, the account was verified within the Users Organizational Unit.

This confirms the employee account was successfully created and is ready for use.

### Procedure

1. Returned to the Users Organizational Unit.
2. Verified Emma Wilson appeared in the directory.

### Result

The employee account was successfully provisioned.

### Screenshot

<img width="755" height="523" alt="ServiceNow Emma Wilson Account Confirmation" src="https://github.com/user-attachments/assets/307e4726-459f-45dd-8bdb-4530e3fc3daf" />

---

# Step 5 - Completing the ServiceNow Request

### Overview

After confirming the account had been created successfully, the ServiceNow request was updated with the work performed and marked as resolved.

Proper documentation provides an audit trail and informs the requester that the onboarding process has been completed.

### Resolution Notes

- Created an Active Directory account for Emma Wilson.
- Assigned a temporary password.
- Enabled the requirement to change the password at first sign-in.
- Configured the employee's job title, department, and organization.
- Verified successful account creation.

### Result

The onboarding request was successfully completed and documented.

### Screenshot

<img width="959" height="920" alt="ServiceNow Emma Wilson Ticket Resolved" src="https://github.com/user-attachments/assets/93e78aca-a06e-4fec-b5b0-8bc0453f895b" />

---

# Summary

This exercise demonstrates the complete onboarding process for a new employee using ServiceNow and Active Directory.

The following tasks were completed:

- Created a ServiceNow onboarding request
- Provisioned a new Active Directory account
- Assigned a temporary password
- Configured employee information
- Verified account creation
- Documented the completed work in ServiceNow
- Successfully resolved the request
