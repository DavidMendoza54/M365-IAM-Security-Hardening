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


