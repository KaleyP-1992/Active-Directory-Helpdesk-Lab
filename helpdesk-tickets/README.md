
# Help Desk Ticket Documentation

## Active Directory Help Desk Home Lab

This folder documents simulated IT Help Desk and Identity and Access Management (IAM) scenarios completed in a Windows Server 2025 Active Directory home lab.

**Environment:**
- Server: PT-DC01
- Domain: helpdesklab.local
- Platform: Oracle VirtualBox
- Technologies: Active Directory, Group Policy, DNS, NTFS, SMB

All users and support requests are fictional and were created for hands-on training.

---

## Ticket #001 — Active Directory User Administration

**Issue:** Establish departmental user accounts and security groups.

**Actions Taken:**
- Created organizational units for HR, Finance, Sales, IT, and Help Desk.
- Created test user accounts in Active Directory.
- Configured departmental security groups.
- Assigned users to their appropriate groups.

**Outcome:** Established a structured Active Directory environment for user and access management.

**Skills:** Active Directory, organizational units, user provisioning, security groups.

---

## Ticket #002 — Account Lockout

**User:** Michael Smith  
**Issue:** Account locked after multiple unsuccessful sign-in attempts.

**Actions Taken:**
- Configured a domain account lockout threshold of five invalid attempts.
- Reproduced an account lockout in the lab.
- Located the user account in Active Directory.
- Unlocked the account without resetting the password.

**Outcome:** Account unlocked successfully. Subsequent sign-in was not independently verified as part of this ticket.

**Skills:** Group Policy, account lockout troubleshooting, Active Directory.

---

## Ticket #003 — Temporary Access Provisioning

**User:** Jessica Rodriguez  
**Issue:** Employee required temporary HR access while remaining in Sales.

**Actions Taken:**
- Reviewed the simulated approved access request.
- Located the user in Active Directory.
- Added the user to GG_HR_Users.
- Verified existing GG_Sales_Users membership remained intact.

**Outcome:** Additional group membership successfully configured.

**Skills:** Access provisioning, role-based access control, IAM.

---

## Ticket #004 — Password Reset

**User:** Sarah Miller  
**Issue:** Employee forgot her password.

**Actions Taken:**
- Simulated identity verification.
- Reset the user's password in Active Directory.
- Enabled the requirement to change the password at next logon.
- Tested authentication with the temporary credentials.

**Outcome:** Password reset completed and authentication tested successfully.

**Skills:** Password administration, account recovery, user support.

---

## Ticket #005 — Employee Offboarding

**User:** Kevin Brooks  
**Issue:** HR requested that a departing employee's account be disabled.

**Actions Taken:**
- Created a simulated Sales employee account.
- Assigned the account to GG_Sales_Users.
- Disabled the account in Active Directory.
- Verified the disabled account indicator.

**Outcome:** Account disabled while retaining its directory object.

**Skills:** Offboarding, account lifecycle management, access security.

---

## Ticket #006 — Temporary Access Removal

**User:** Jessica Rodriguez  
**Issue:** Temporary HR project completed; additional access no longer required.

**Actions Taken:**
- Located the user's security group memberships.
- Removed GG_HR_Users membership.
- Retained GG_Sales_Users membership.
- Verified the updated group configuration.

**Outcome:** Temporary group access removed successfully.

**Skills:** Access deprovisioning, least privilege, IAM.

---

## Ticket #007 — New Employee Onboarding

**User:** Emily Carter  
**Department:** Finance

**Actions Taken:**
- Created an Active Directory user account.
- Assigned the account to the Finance organizational unit.
- Added the user to GG_Finance_Users.
- Required a password change at next logon.

**Outcome:** New account provisioned with the intended Finance group membership.

**Skills:** User onboarding, Active Directory, group management.

---

## Ticket #008 — Department Transfer

**User:** Emily Carter  
**Issue:** Employee transferred from Finance to HR.

**Actions Taken:**
- Moved the account from the Finance OU to the HR OU.
- Removed GG_Finance_Users membership.
- Added GG_HR_Users membership.

**Outcome:** Directory placement and group memberships updated for the new department.

**Skills:** Account lifecycle management, access changes, least privilege.

---

## Ticket #009 — Finance Shared Folder Access

**User:** Michael Smith  
**Issue:** Employee reported difficulty accessing Finance resources.

**Actions Taken:**
- Verified membership in GG_Finance_Users.
- Configured NTFS Modify permissions for the Finance group.
- Configured the FinanceShare network share.
- Investigated Windows logon restrictions on the domain controller.
- Mapped the share using explicit domain credentials.
- Successfully listed the shared folder's contents.

**Outcome:** Network share mapping and read access verified using the supplied domain credentials. Write access and unauthorized-user denial were not separately tested.

**Skills:** NTFS permissions, SMB sharing, authentication troubleshooting, drive mapping.

---

## Project Summary

These nine simulated scenarios provided hands-on experience with common IT Help Desk responsibilities, including:

- User account administration
- Password resets and account lockouts
- Employee onboarding and offboarding
- Access provisioning and deprovisioning
- Group Policy configuration
- File-sharing permissions
- Troubleshooting and documentation

**Note:** All work was performed in a personal lab environment for educational and portfolio purposes.
