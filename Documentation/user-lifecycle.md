# User Lifecycle Management

## Purpose 

This document outlines a user lifecycle management process for a Microsoft 365 environment. The goal is to make sure users receive the correct access when they join, change roles, or leave the organization.

User lifecycle management is important because identity security does not stop after an account is created. Access must be reviewed, updated, and removed throughout a user's time with the organization.

This project is written as a portfolio case study and does not include real tenant names, usernames, domains, email addresses, or confidential information.

## Lifecycle Overview

User lifecycle management includes three major stages:

1. Onboarding
2. Role Changes
3. Offboarding

Each stage should follow a documented process to reduce security risk, prevent unnecessary access, and improve accountability.

## Security Goals

- Assign access based on job role and business need
- Apply least privilege during onboarding
- Review and update access when users change roles
- Remove access quickly when users leave
- Reduce stale accounts and privilege creep
- Improve accountability through documented access decisions
- Protect Microsoft 365 data, email, files, and applications

## Key User Lifecycle Risks

|Risk|Impact|Recommended Control|
| --- | --- | --- |
|New users receive too much access|Increases risk of unauthorized data exposure|Assign access based on role and least privilege|
|Role changes are not reviewed|Users may keep old permissions they no longer need|Review access during department or responsibility changes|
|Former users retain access|Unauthorized access after departure|Disable accounts immediately during offboarding|
|Shared accounts are used|Reduces accountability and auditing|Use named accounts whenever possible|
|Licenses are not removed|Wastes resources and may leave access active|Remove or reassign licenses during offboarding|
|Mailbox access is not reviewed|Former or incorrect users may access sensitive email|Review mailbox permissions and shared mailbox access|

## Onboarding Process

The onboarding process should ensure that new users receive the correct access based on their job responsibilities.

### Recommended onboarding steps:

- Create a named user account
- Assign the correct Microsoft 365 license
- Add the user to approved groups based on role
- Require Multi-Factor Authentication registration
- Provide access to email, Teams, SharePoint, and required applications
- Avoid assigning admin roles unless approved
- Document access granted during onboarding
- Provide basic cybersecurity awareness guidance

## Role Change Process

When a user changes departments, responsibilities, or job roles, their access should be reviewed. This helps prevent privilege creep, where users slowly collect access they no longer need.

### Recommended role change steps:

- Review the user's current groups, roles, and permissions
- Review the user's current groups, roles, and permissions
- Assign new access based on the updated role
- Review shared mailbox permissions
- Review shared mailbox permissions
- Confirm administrative access is still justified
- Document all access changes

## Ofboarding Process

The offboarding process should remove access quickly and safely when a user leaves the organization. This is one of the most important identity security controls because former users should not retain access to email, files, systems, or cloud applications.

### Recommended offboarding steps:

- Disable the user account
- Revoke active sessions
- Reset the password if needed
- Remove or reassign Microsoft 365 license
- Remove user from groups and roles
- Remove administrative access
- Convert mailbox to shared mailbox if needed
- Configure mailbox delegation or forwarding only if approved
- Transfer OneDrive or file ownership if needed
- Document completion of offboarding tasks

## Access Review Process

Access reviews should be performed regularly to confirm that users still need their assigned permissions.

### Recommended review items:

- Inactive accounts
- Users with admin roles
- Shared mailbox permissions
- Microsoft 365 group memberships
- SharePoint and Teams access
- Guest or external users
- Users with licenses but no recent activity
- Accounts with failed or suspicious sign-in activity

