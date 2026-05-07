# Identity and Access Management (IAM) Solutions

## Overview

Identity and Access Management (IAM) is a security framework that ensures the right individuals access the right resources at the right time and for the right reasons.

IAM helps organizations manage:

- User identities
- Authentication
- Access permissions
- Security monitoring

---

## Core IAM Components

Common IAM components include:

- Password Management
- Network Access Control (NAC)
- Digital Identity Management

---

## IAAA Model

IAM commonly follows the **IAAA model**.

---

## 1. Identification

Identification is the process where a user claims an identity.

### Common Examples

- Username
- Email address
- Employee ID

### Purpose

Allow the system to recognize who is requesting access.

---

## 2. Authentication

Authentication verifies whether the claimed identity is valid.

### Common Authentication Methods

- Passwords
- Biometrics
- Tokens
- Multi-Factor Authentication (MFA)

### Purpose

Verify user identity before access is granted.

---

## 3. Authorization

Authorization determines what resources an authenticated user can access.

### Common Authorization Models

- Role-Based Access Control (RBAC)
- Attribute-Based Access Control (ABAC)
- Access Control Lists (ACLs)

### Purpose

Enforce least privilege and access boundaries.

---

## 4. Accounting

Accounting records user actions and access activities.

### Common Examples

- Login logs
- Access records
- Administrative changes
- Security events

### Purpose

Provide accountability, auditing, and forensic visibility.

---

## IAM Concepts

## Provisioning

Provisioning is the process of creating new user accounts and assigning appropriate access rights.

### Common Tasks

- Account creation
- Role assignment
- Group membership
- Resource allocation

---

## Deprovisioning

Deprovisioning removes access when users no longer require it.

### Important Security Goal

Prevent **orphaned accounts**.

Orphaned accounts may become security risks if not removed.

---

## Identity Proofing

Identity proofing verifies a user's real-world identity before granting access.

### Common Methods

- Government identification
- Employee verification
- Background verification

---

## Interoperability

Interoperability allows identity information to be shared securely across different systems.

### Common Standards

- SAML
- OAuth
- OpenID Connect

---

## Attestation

Attestation is the periodic review of user access rights.

### Purpose

Prevent **privilege creep**.

Privilege creep occurs when users accumulate unnecessary permissions over time.

---

# Multi-Factor Authentication (MFA)

MFA uses multiple independent authentication factors.

---

## Authentication Factors

### Something You Know

Examples:

- Password
- PIN

---

### Something You Have

Examples:

- Smart card
- Security token
- Mobile phone

---

### Something You Are

Examples:

- Fingerprint
- Facial recognition
- Retina scan

---

### Somewhere You Are

Examples:

- GPS location
- IP address

---

### Something You Do

Examples:

- Typing patterns
- Behavioral biometrics

---

## Authentication Types

| Type | Description |
|------|-------------|
| **Single-Factor Authentication** | Uses one authentication factor |
| **Two-Factor Authentication (2FA)** | Uses two different factors |
| **Multi-Factor Authentication (MFA)** | Uses two or more factors |

---

## Common MFA Technologies

Examples include:

- Biometric systems
- Hardware tokens
- Software tokens
- Security keys
- Passkeys

---

## Password Security

Strong password security remains essential.

---

## Password Policy Elements

Organizations commonly enforce:

- Minimum length (12–16+ characters recommended)
- Complexity requirements
- Password reuse restrictions
- Expiration policies
- Minimum password age

---

## Password Managers

Password managers help users:

- Generate strong passwords
- Store credentials securely
- Auto-fill credentials
- Synchronize across devices
- Share credentials securely

---

## Passwordless Authentication

Modern authentication may eliminate traditional passwords.

### Common Methods

- Biometrics
- Hardware security keys
- One-Time Passwords (OTP)
- Magic links
- Passkeys

---

## Password Attacks

## Brute Force Attack

Attempts all possible combinations.

### Mitigation

- MFA
- Login attempt limits
- Strong passwords

---

## Dictionary Attack

Uses common password lists.

### Mitigation

- Password complexity
- MFA
- Account lockout policies

---

## Password Spraying

Attempts a small number of common passwords across many accounts.

### Mitigation

- Unique passwords
- Lockout controls
- Monitoring

---

## Hybrid Attack

Combines dictionary attacks with brute force techniques.

### Mitigation

- Longer passwords
- MFA

---

# Single Sign-On (SSO)

SSO allows users to authenticate once and access multiple systems.

---

## Benefits

- Improved user experience
- Fewer password resets
- Centralized authentication
- Stronger policy enforcement

---

## Common SSO Technologies

- LDAP
- OAuth
- SAML
- OpenID Connect

---

# Federation

Federation allows identity sharing between organizations or systems.

---

## Federation Process

1. User requests access to a service provider (SP)
2. The service provider redirects the user to an identity provider (IdP)
3. The identity provider authenticates the user
4. The identity provider creates an assertion or token
5. The token is sent back to the service provider
6. The service provider validates the token
7. Access is granted

---

# Privileged Access Management (PAM)

PAM controls and monitors privileged accounts.

---

## Common PAM Features

### Just-In-Time (JIT) Permissions

Temporary elevated access for specific tasks.

---

### Password Vaulting

Secure storage and auditing of administrative credentials.

---

### Temporal Accounts

Accounts created for temporary access periods.

---

# Access Control Models

## Mandatory Access Control (MAC)

Security is enforced using labels or classifications.

### Characteristics

- Highly secure
- Users cannot change permissions

---

## Discretionary Access Control (DAC)

Resource owners control permissions.

### Characteristics

- Flexible
- Less secure than MAC

---

## Role-Based Access Control (RBAC)

Permissions are assigned based on job roles.

### Characteristics

- Most common enterprise model
- Supports least privilege

---

## Rule-Based Access Control

Access decisions are based on defined rules or policies.

---

## Attribute-Based Access Control (ABAC)

Access decisions are based on attributes such as:

- User attributes
- Resource attributes
- Environmental conditions

---

# Access Control Extensions

## Time-Based Restrictions

Access is limited to specific hours or schedules.

---

## Least Privilege

Users receive only the permissions required for their job.

---

## Group Permissions

Permissions assigned to groups are inherited by members.

---

## File and Folder Permissions

Operating systems allow access control on files and directories.

Examples include:

- Read
- Write
- Execute
- Modify

---

## Important Exam Concepts

| Scenario | Best Answer |
|----------|--------------|
| Verify identity | Authentication |
| Determine access rights | Authorization |
| Record user activity | Accounting |
| Temporary admin privileges | JIT |
| Excessive permission accumulation | Privilege Creep |
| Single login across systems | SSO |
| Cross-organization identity sharing | Federation |
| Role-based permissions | RBAC |

---

## Summary

IAM helps organizations:

- Verify user identities
- Control resource access
- Monitor user activity
- Reduce unauthorized access risks
- Enforce least privilege

IAM works together with:

- MFA
- Password policies
- SSO
- PAM
- Access control models

To provide secure identity and access management.

---
