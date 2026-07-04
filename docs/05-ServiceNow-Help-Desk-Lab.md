# ServiceNow Help Desk Lab

## Objective

The goal of this section is to simulate a real-world Help Desk workflow by creating and resolving an incident using ServiceNow and Active Directory.

The scenario demonstrates a common IT support task where a user's Active Directory account becomes locked after multiple failed login attempts. The incident is documented in ServiceNow, resolved using Active Directory Users and Computers (ADUC), and then closed after confirming the issue has been resolved.

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

# Help Desk Scenario

**User:** Mason Reed

**Issue Reported:** Unable to log into the company computer after multiple failed password attempts.

**Objective:** Reset the user's password, unlock the Active Directory account, document all actions performed, and successfully resolve the ServiceNow incident.

---

# Step 1 - Creating a ServiceNow Incident

### Overview

A new incident was created in ServiceNow to simulate a Help Desk support request.

The incident records important information such as the affected user, issue description, priority, assignment group, and work notes.

### Procedure

1. Logged into the ServiceNow Developer Instance.
2. Navigated to **Incidents**.
3. Selected **Create New**.
4. Entered the user's information.
5. Documented the reported issue.
6. Submitted the incident.

### Result

A new Help Desk incident was successfully created and assigned an incident number for tracking.

### Screenshot

<img width="957" height="639" alt="ServiceNow Ticket Creation Mason Reed" src="https://github.com/user-attachments/assets/85f6a54f-15ad-45a7-9784-6cf971db07a9" />

---

# Step 2 - Viewing the Incident Queue

### Overview

After creating the incident, it appeared in the list of active incidents.

The incident queue allows Help Desk technicians to view, prioritize, and manage support requests.

### Procedure

1. Opened the **Incident List**.
2. Located the newly created incident.

### Result

The new incident appeared successfully within the ServiceNow incident queue.

### Screenshot

<img width="956" height="803" alt="ServiceNow List of Incidents " src="https://github.com/user-attachments/assets/d79b8f39-3d12-4aa0-8206-c71eeb805d95" />

---

# Step 3 - Reviewing the Incident

### Overview

The incident was opened to review the reported issue before beginning troubleshooting.

Reviewing the incident ensures the technician understands the user's problem before making any changes.

### Procedure

1. Opened the incident.
2. Reviewed the caller information.
3. Read the incident description.
4. Confirmed the reported issue.

### Result

The incident was ready for investigation and resolution.

### Screenshot

<img width="957" height="912" alt="ServiceNow Mason Reed Open ticket" src="https://github.com/user-attachments/assets/fa0097ad-7a0d-4aca-8a25-b465acd4e267" />

---

# Step 4 - Resetting the User Password in Active Directory

### Overview

The affected user's account was located in Active Directory Users and Computers.

The account was unlocked and the password was reset to restore access.

Password resets and account unlocks are among the most common tasks performed by Help Desk technicians.

### Procedure

1. Opened **Active Directory Users and Computers**.
2. Located the user account.
3. Right-clicked the user.
4. Selected **Reset Password**.
5. Assigned a temporary password.
6. Unlocked the account.
7. Enabled **User must change password at next logon**.

### Result

The user's account was successfully unlocked and the password was reset.

### Screenshot

<img width="756" height="499" alt="Azure VM AD USER PASSWORD RESET" src="https://github.com/user-attachments/assets/7599c3f7-6474-48c4-8b26-adff9b962e29" />
<img width="757" height="497" alt="Azure VM AD USER PASSWORD RESET CONFIRMATION" src="https://github.com/user-attachments/assets/0a6500d6-9ad9-461a-8125-0ec3ed74c751" />

---

# Step 5 - Documenting the Resolution

### Overview

After resolving the issue, detailed work notes were added to the ServiceNow incident.

Accurate documentation allows future technicians to understand what actions were performed and provides an audit trail for support requests.

### Example Work Notes

- Verified the user's identity.
- Located the user account in Active Directory.
- Reset the account password.
- Unlocked the account.
- Instructed the user to change the temporary password after logging in.

### Procedure

1. Returned to ServiceNow.
2. Entered work notes describing the actions performed.
3. Updated the incident.

### Result

The incident history now contains a complete record of the troubleshooting process.

### Screenshot

<img width="955" height="915" alt="ServiceNow Ticket Mason Reed resolved" src="https://github.com/user-attachments/assets/15243e39-d293-460c-a0a7-63b24ad247cd" />

---

# Step 6 - Resolving the Incident

### Overview

After confirming the user could successfully sign in, the incident was marked as resolved.

Closing incidents after verifying successful resolution ensures the ticket lifecycle is completed properly.

### Procedure

1. Confirmed the user's issue had been resolved.
2. Updated the incident state to **Resolved**.
3. Added the resolution notes.
4. Saved the incident.

### Result

The incident was successfully resolved and removed from the list of active support requests.

### Screenshot

<img width="956" height="356" alt="ServiceNow Mason Reed ticket resolved confirmation" src="https://github.com/user-attachments/assets/e3934c57-9ed9-40f3-aaaa-157be5d668d6" />

---

# Summary

This lab demonstrates a complete Help Desk support workflow using both ServiceNow and Active Directory.

The following tasks were successfully completed:

- Created a ServiceNow incident
- Reviewed the support request
- Located the affected user in Active Directory
- Reset the user's password
- Unlocked the user account
- Documented all actions performed
- Successfully resolved the ServiceNow incident

This exercise closely reflects the daily responsibilities of Help Desk Technicians and IT Support Specialists working in enterprise environments.
