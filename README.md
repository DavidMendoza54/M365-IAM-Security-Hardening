# Microsoft 365 IAM Security Hardening

## Overview

This project is a Microsoft 365 Identity and Access Management security hardening case study. The goal is to document how an organization can strengthen account security, reduce unauthorized access, and improve identity protection using Microsoft 365 and Microsoft Entra ID security principles.

The project focuses on Multi-Factor Authentication, Conditional Access, Role-Based Access Control, least privilege, privileged access management, user lifecycle management, and security monitoring.

## Project Objectives

- Strengthen identity security in a Microsoft 365 environment
- Reduce account compromise risk through MFA and access controls
- Apply least privilege and Role-Based Access Control principles
- Improve onboarding, offboarding, and user lifecycle management
- Document privileged access risks and mitigation strategies
- Align identity security practices with Zero Trust concepts

## Security Areas Covered

- Identity and Access Management
- Multi-Factor Authentication
- Conditional Access
- Role-Based Access Control
- Least Privilege
- Privileged Access Management
- User Provisioning and Deprovisioning
- Account Security
- Cloud Security
- Microsoft 365 Security Administration


## Design Approach

The identity security model is built around the idea that user accounts are one of the most common attack targets in a cloud environment. If an attacker compromises an account, they may be able to access email, files, administrative portals, cloud applications, and sensitive organizational data.

To reduce this risk, the environment should enforce strong authentication, limit administrative privileges, monitor risky sign-ins, and ensure user access is removed when it is no longer needed.

This project documents a practical security hardening approach for Microsoft 365 environments, especially small to mid-sized organizations that may not have a dedicated security team.

## Security Design Decisions

|Design Decision|Reason|
| ----------- | ----------- |
|Require MFA for users and administrators|Reduces the risk of account compromise from stolen passwords.|
|Apply least privilege access|Limits damage if an account is compromised.|
|Separate standard user accounts from admin accounts|Reduces unnecessary exposure of privileged access.|
|Review privileged roles regularly|Helps prevent privilege creep and unused admin access.|
|Create an onboarding and offboarding process|Ensures users receive proper access and lose access when they leave.|
|Monitor sign-in activity and risky behavior|Improves detection of suspicious account activity.|

## Project Files 

- [iam-security-plan.md](Documentation/iam-security-plan.md) - Identity security hardening plan
- [user-lifecycle.md](Documentation/user-lifecycle.md) - Onboarding, role changes, and offboarding process
- [rbac-model.md](Documentation/rbac-model.md) - Administrative role and privileged access plan
- [mfa-conditional-access-plan.md](Documentation/mfa-conditional-access-plan.md) - Conditional Access and MFA policy planning
- [Diagrams](Diagrams/) - IAM security flow diagrams
