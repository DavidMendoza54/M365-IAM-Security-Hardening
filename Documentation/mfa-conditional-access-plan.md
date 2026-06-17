# MFA and Conditional Access Plan

## Purpose

This document outlines a Multi-Factor Authentication and Conditional Access plan for a Microsoft 365 environment. The goal is to reduce account compromise risk, enforce stronger sign-in requirements, and apply access controls based on user role, risk level, device trust, and application sensitivity.

This project is written as a portfolio case study and does not include real tenant names, usernames, domains, IP addresses, policy names, or confidential information.

## Secuirty Goals

- Require MFA for users and administrators
- Protect privileged accounts with stronger authentication requirements
- Reduce risk from stolen or reused passwords
- Block or limit insecure sign-in methods
- Apply access controls based on user, device, location, application, and risk
- Support Zero Trust principles by verifying access before allowing it

## Why MFA Matters

Passwords alone are not enough to protect cloud accounts. Users may reuse passwords, fall for phishing attempts, or have credentials exposed in a data breach. Multi-Factor Authentication adds another layer of protection by requiring an additional verification method before access is granted.

For administrators, MFA is especially important because compromised privileged accounts can lead to major security incidents, data exposure, or tenant-wide changes.

## Conditional Access Overview 

Conditional Access policies help enforce security decisions during sign-in. Instead of treating every login the same, access decisions can be based on conditions such as:

- User or group membership
- Administrator role
- Device compliance or trust level
- Location or sign-in risk
- Application being accessed
- Authentication strength

This allows the organization to apply stronger controls to higher-risk situations.

# Recommended Conditional Access Policies

|Policy|Target|Control|Access Policies|
| --- | --- | --- | --- |
|Require MFA for administrators|Admin roles|Require MFA|Protects high-privilege accounts from unauthorized access|
|Require MFA for all users|Standard users|Require MFA|Reduces account compromise risk|
|Block legacy authentication|All users|Block access|Prevents older protocols from bypassing modern authentication controls|
|Require MFA for risky sign-ins|Users with unusual or risky login behavior|Require MFA|Adds protection when sign-in behavior appears suspicious|
|Restrict access to sensitive apps|Users accessing sensitive Microsoft 365 apps|Require MFA or trusted device|Protects email, files, and administrative portals|
|Monitor unfamiliar locations|Users signing in from unusual locations|Require MFA or review|Helps detect potentially suspicious account activity|

## Admin Account Protection

Administrative accounts should have stronger access requirements than standard user accounts.

Recommended controls:

- Require MFA for all admin accounts
- Limit Global Administrator access
- Use least privilege role assignments
- Separate daily-use accounts from admin accounts when possible
- Monitor admin sign-in activity
- Monitor admin sign-in activity

## Legacy Authentication Risk
