# Active Directory Help Desk Home Lab

## Project Overview

This project demonstrates the deployment and administration of a Windows Server 2025 Active Directory environment using Oracle VirtualBox.

I created this home lab to develop practical IT Help Desk, system administration, and identity and access management (IAM) skills. The environment simulates common workplace IT support requests, including password resets, account lockouts, employee onboarding, offboarding, and access management.

## Technologies Used

- Windows Server 2025
- Oracle VirtualBox
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy Management
- NTFS and SMB File Sharing
- Windows Command Prompt

## Lab Environment

| Component | Configuration |
|---|---|
| Server Name | PT-DC01 |
| Domain | helpdesklab.local |
| Operating System | Windows Server 2025 |
| Virtualization | Oracle VirtualBox |
| Organizational Units | HR, Finance, Sales, IT, Help Desk |

## Project Implementation

### 1. Windows Server Deployment
Installed Windows Server 2025 in VirtualBox, configured networking, and prepared the server for domain administration.

### 2. Active Directory Configuration
Installed Active Directory Domain Services, promoted the server to a domain controller, and created the `helpdesklab.local` domain.

### 3. User and Group Management
Created departmental organizational units, user accounts, and security groups to simulate an enterprise environment.

### 4. Group Policy Configuration
Configured an account lockout policy that locks accounts after five invalid sign-in attempts.

### 5. Help Desk Troubleshooting
Practiced resolving common IT support issues involving user authentication, password management, and account permissions.

### 6. File Sharing and Permissions
Created a Finance network share, configured NTFS and share permissions, and tested access using domain credentials.

## Help Desk Scenarios

| Ticket | Scenario |
|---|---|
| #001 | Active Directory user administration |
| #002 | Account lockout troubleshooting |
| #003 | Temporary departmental access |
| #004 | Password reset |
| #005 | Employee offboarding |
| #006 | Access removal |
| #007 | New employee onboarding |
| #008 | Department transfer |
| #009 | Finance shared folder access troubleshooting |


📋 [View All Nine Help Desk Tickets](helpdesk-tickets/README.md)


These scenarios were performed in a simulated lab environment.

## Skills Demonstrated

- Windows Server installation and administration
- Active Directory user and group management
- Organizational Unit administration
- Password resets and account unlocks
- Group Policy configuration
- Identity and access management
- Employee onboarding and offboarding
- NTFS and network share permissions
- Windows command-line troubleshooting
- Technical documentation

## Project Screenshots

The repository includes 13 screenshots documenting the Windows Server deployment, Active Directory configuration, account management, Group Policy, and network-share troubleshooting.

## Key Takeaways

This project strengthened my understanding of how Active Directory supports enterprise IT operations. I gained hands-on experience managing user identities, assigning access through security groups, troubleshooting authentication issues, and documenting Help Desk procedures.

## Future Improvements

- Automate Active Directory tasks using PowerShell.
- Add a domain-joined Windows client for end-user testing.
- Expand security monitoring and auditing capabilities.

- ## Lab Screenshots

### 1. Virtual Machine Creation
![Virtual Machine Creation](01-VM%20Creation.png)


### 2. Windows Server Manager
![Windows Server Manager](02-Server%20Manager.png)

### 3. Active Directory Domain
![Active Directory Domain](03-Active%20Directory%20Domain.png)

### 4. Organizational Units
![Organizational Units](04-Organizational%20Units.png)

### 5. User Accounts
![User Accounts](05-User%20Accounts.png)

### 6. Security Groups
![Security Groups](06-Security%20Groups.png)

### 7. Group Memberships
![Group Memberships](07-Group%20Memberships.png)

### 8. Account Lockout Policy
![Account Lockout Policy](08-Account%20Lockout%20Policy.png)

### 9. Disabled Employee Account
![Disabled Account](09-Disabled%20Account.png)

### 10. Finance NTFS Permissions
![Finance NTFS Permissions](10-Finance%20NTFS.png)

### 11. Finance Network Share Permissions
![Finance Sharing](11-Finance%20Sharing.png)

### 12. Finance Network Drive
![Finance Drive](12-Finance%20Drive.png)

### 13. Finance Shared Folder Access
![Finance Access](13-Finance%20Access.png)

