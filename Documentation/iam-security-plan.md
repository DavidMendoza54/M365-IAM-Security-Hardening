## IAM Security Plan

# Purpose
This document outlines an Identity and Access Management security plan for a Microsoft 365 environment. The goal is to reduce account compromise risk, strengthen authentication, limit unnecessary access, and improve visibility into identity-related activity.

This project is written as a portfolio case study and does not include real tenant names, usernames, domains, IP addresses, or confidential information.

# Security Goals
- Require strong authentication for users and administrators
- Reduce risk from stolen, reused, or weak passwords
- Apply least privilege across user and administrator roles
- Separate standard user access from privileged administrative access
- Improve onboarding, role change, and offboarding processes
- Monitor sign-in activity and identity-related security events
- Support Zero Trust principles by verifying access instead of automatically trusting it

# IAM Hardening Checklist

Control|Priority|
| --- | --- |
|Require MFA for all administrators|High|
|Require MFA for all users|High|
|Disable legacy authentication|High|
|Review Global Administrator assignments|High|
|Create user onboarding checklist|Medium|
|Create user offboarding checklist|Medium|
|Review sign-in logs regularly|Medium|
|Document privileged role assignments|Medium|
|Review inactive accounts|Medium|
|Monitor MFA registration changes|Medium|