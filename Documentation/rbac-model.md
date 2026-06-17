# Privileged Access and RBAC Model

## Purpose 

This document outlines a Role-Based Access Control model for a Microsoft 365 environment. The goal is to reduce unnecessary administrative access, apply least privilege, improve accountability, and protect privileged accounts from compromise.

This project is written as a portfolio case study and does not include real tenant names, usernames, domains, admin accounts, or confidential information.

## RBAC Overview

Role-Based Access Control is a security model where access is assigned based on a user’s job responsibilities. Instead of giving broad permissions to every user, permissions are assigned based on what each role needs to perform its work.

In a Microsoft 365 environment, RBAC helps control access to services such as Microsoft Entra ID, Exchange Online, SharePoint, Teams, security portals, and administrative settings.

## Security Goals

- Apply least privilege to all users and administrators
- Limit Global Administrator access
- Separate daily-use accounts from privileged admin accounts
- Assign permissions based on job responsibility
- Review privileged roles regularly
- Reduce privilege creep over time
- Improve accountability and auditability

## Key RBAC Risks

|Risk|Impact|Recommended Control|
| --- | --- | --- |
|Too many Global Administrators|A compromised admin account could lead to tenant-wide impact|Limit Global Administrator roles to only approved users|
|Privilege creep|Users keep access they no longer need after role changes|Perform scheduled access reviews|
|Shared admin accounts|Makes it difficult to identify who made changes|Use named admin accounts|
|Admin accounts used for daily work|Increases exposure through email, browsing, and phishing|Use separate admin accounts|
|Unreviewed role assignments|Old or unnecessary permissions remain active|Document and review privileged roles|Review admin sign-ins and audit logs|


## Recommended Role Model
|Role Type|Example Responsibility|Access Recommendation|
| --- | --- | --- |
|Standard User|Email, Teams, OneDrive, SharePoint access|No administrative privileges|
|Help Desk / Support|Password resets, basic user support, MFA assistance|Limited help desk roles only|
|Exchange Admin|Mailbox management, shared mailboxes, mail flow settings|Exchange-specific admin role|
|Exchange Admin|SharePoint sites, permissions, and storage management|SharePoint-specific admin role|
|Security Admin|Security alerts, policies, and security settings|Security-focused admin role|
|Global Administrator|Tenant-wide emergency or high-level administration|Highly restricted and reviewed regularly|

## Least Privilege Approach

Users and administrators should only receive the permissions needed to perform their responsibilities. Broad administrator roles should be avoided unless there is a clear business need.

### Recommended actions:

- Assign service-specific roles instead of Global Administrator when possible
- Document why each privileged role is needed
- Remove access when users change roles
- Review privileged roles on a scheduled basis
- Avoid assigning admin access permanently unless required
- Use separate admin accounts for privileged work when possible

## Global Administrator Protection

Global Administrator access should be treated as the highest-risk role in the environment because it can make major tenant-wide changes.

### Recommended protections:

- Limit the number of Global Administrators
- Require MFA for every Global Administrator account
- Review Global Administrator assignments regularly
- Review Global Administrator assignments regularly
- Monitor Global Administrator sign-ins
- Keep emergency access accounts protected and documented

## Admin Account Seperation

Administrative users should use standard accounts for daily work and separate admin accounts for privileged tasks. This reduces the chance that privileged access is exposed through normal user activity such as email, web browsing, or general application use.

### Example:

|Account Type|Purpose|
| --- | --- |
|Standard Account|Daily work such as email, Teams, SharePoint, and normal activity|
|Admin Account|Privileged administrative tasks only|

## Access Review Process

Privileged access should be reviewed regularly to confirm that each admin role is still needed.

### Recommended access review questions:

- Does this user still need this role?
- Is this the lowest privilege role that meets the need?
- Is the role assigned to a named account?
- Is MFA enabled for the account?
- Has the user changed job responsibilities?
- Is there documentation explaining why access is needed?

## Example Implementation Phases

### Phase 1: Review Current Access

Review all administrative roles, Global Administrator assignments, shared admin accounts, inactive accounts, and users with elevated permissions.

### Phase 2: Reduce Excessive Privileges

Remove unnecessary admin access, replace broad roles with service-specific roles, and document approved privileged users.

### Phase 3: Strengthen Admin Account Security

Require MFA for privileged accounts, separate admin accounts from daily-use accounts, and monitor admin sign-ins.

### Phase 4: Ongoing Review

Create a recurring access review process to reduce privilege creep and keep role assignments accurate over time.
