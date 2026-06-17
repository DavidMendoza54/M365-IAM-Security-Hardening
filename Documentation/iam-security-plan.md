# IAM Security Plan

## Purpose

This document outlines an Identity and Access Management security plan for a Microsoft 365 environment. The goal is to reduce account compromise risk, strengthen authentication, limit unnecessary access, and improve visibility into identity-related activity.

This project is written as a portfolio case study and does not include real tenant names, usernames, domains, IP addresses, or confidential information.

## Security Goals

- Require strong authentication for users and administrators
- Reduce risk from stolen, reused, or weak passwords
- Apply least privilege across user and administrator roles
- Separate standard user access from privileged administrative access
- Improve onboarding, role change, and offboarding processes
- Monitor sign-in activity and identity-related security events
- Support Zero Trust principles by verifying access instead of automatically trusting it

## Microsoft 365 IAM Hardening Recommendations

|Area|Recommendation|Security Benefit|
| --- | --- | --- |
|MFA|Require MFA for all users and administrators|Reduces account compromise risk if passwords are stolen|
|Admin Access|Limit Global Administrator roles and use least privilege|Reduces damage from compromised admin accounts|
|Legacy Authentication|Block legacy authentication protocols where possible|Prevents older sign-in methods from bypassing modern security controls|
|User Lifecycle|Create onboarding, role change, and offboarding checklists|Ensures users have correct access and lose access when they leave|
|Sign-In Monitoring|Review failed logins, risky sign-ins, and unusual locations|Improves detection of suspicious account activity|
|Shared Accounts|Replace shared accounts with named accounts when possible|Improves accountability and auditing|
|Access Reviews|Review privileged roles and inactive accounts regularly|Reduces privilege creep and stale access|

## IAM Hardening Checklist

Control|Priority|
| :--- | :---: |
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

## Implementation Phases

### Phase 1: Assessment 

Review current users, administrator roles, MFA registration, shared accounts, inactive accounts, and sign-in activity.

### Phase 2: Security Hardening

Strengthen MFA, reduce unnecessary admin access, disable legacy authentication, and document Conditional Access recommendations.

### Phase 3: Lifecycle Management

Create onboarding, role change, and offboarding procedures to keep access accurate over time.

### Phase 4: Monitor and Review

Establish a regular review process for sign-ins, risky activity, privileged roles, inactive accounts, and security recommendations.
