# Security Controls

## Security Control Categories

Security controls can be categorized based on how they are implemented.

---

## 1. Managerial Controls

Managerial controls focus on governance, policies, planning, and risk management.

These controls guide people and organizational processes rather than directly enforcing technology.

### Common Examples

- Risk assessments
- Security policies
- Security awareness training
- Compliance programs
- Business continuity planning

### Purpose

- Define security expectations
- Support governance
- Reduce organizational risk

---

## 2. Operational Controls

Operational controls are implemented through daily business operations and human processes.

These controls help ensure systems remain secure during normal operations.

### Common Examples

- Patch management
- Data backups
- Incident response procedures
- Security monitoring
- User onboarding and offboarding

### Purpose

- Maintain operational security
- Support daily security activities
- Improve process consistency

---

## 3. Technical Controls

Technical controls are implemented using hardware or software technologies.

These controls are often enforced automatically by systems.

### Common Examples

- Firewalls
- Intrusion Detection Systems (IDS)
- Intrusion Prevention Systems (IPS)
- Encryption
- Antivirus solutions
- Endpoint Detection and Response (EDR)

### Purpose

- Enforce security policies
- Detect malicious activity
- Prevent unauthorized access

---

## Security Controls by Function

Security controls may also be categorized by their purpose.

---

## Preventive Controls

Preventive controls stop security incidents before they occur.

### Examples

- Firewalls
- Multi-Factor Authentication (MFA)
- Encryption
- Access control systems

### Purpose

Prevent unauthorized actions before damage occurs.

---

## Detective Controls

Detective controls identify suspicious or malicious activity after it occurs.

### Examples

- IDS
- CCTV systems
- Log monitoring
- Security alerts

### Purpose

Detect incidents as quickly as possible.

---

## Corrective Controls

Corrective controls restore systems after an incident.

### Examples

- Security patches
- Backup restoration
- Disaster Recovery Plans (DRP)

### Purpose

Recover from incidents and restore normal operations.

---

## Deterrent Controls

Deterrent controls discourage attackers from attempting malicious actions.

### Examples

- Warning signs
- Security lighting
- Security guards
- Visible surveillance systems

### Purpose

Discourage attacks before they begin.

---

## Compensating Controls

Compensating controls provide alternative protection when primary controls are not available.

### Examples

- UPS systems
- Network segmentation
- Sandboxing
- Additional monitoring controls

### Purpose

Reduce risk when ideal controls cannot be implemented.

---

## Directive Controls

Directive controls guide behavior through rules and policies.

### Examples

- Acceptable Use Policy (AUP)
- Incident Response Policy (IRP)
- Security procedures
- Standard Operating Procedures (SOP)

### Purpose

Define expected behavior and security requirements.

---

## AAA (Authentication, Authorization, Accounting)

AAA is a security framework used to control access and track activity.

---

## Authentication

Authentication verifies the identity of a user, system, or device.

### Common Examples

- Username and password
- Biometrics
- Smart cards
- Multi-Factor Authentication (MFA)

### Purpose

Confirm identity before granting access.

---

## Authorization

Authorization determines what resources an authenticated entity can access.

### Examples

- File permissions
- Role-Based Access Control (RBAC)
- Privileged access management

### Purpose

Enforce least privilege.

---

## Accounting

Accounting records user actions and resource usage.

### Examples

- Login logs
- Access logs
- Administrative activity logs

### Purpose

Provide visibility, accountability, and auditability.

---

## AAA Protocols

### RADIUS

Remote Authentication Dial-In User Service is commonly used for:

- VPN authentication
- Wireless authentication
- Network access control

### Key Features

- Supports AAA
- Uses UDP
- Widely supported

---

## TACACS+

Terminal Access Controller Access-Control System Plus is commonly used for:

- Network device administration
- Privileged administrative access

### Key Features

- Supports AAA
- Uses TCP
- Separates authentication, authorization, and accounting

---

## Authentication-Only Protocols

The following protocols mainly provide authentication:

- PAP
- CHAP
- MS-CHAP

These do not provide full AAA functionality.

---

## Non-Repudiation

Non-repudiation ensures that a user cannot deny performing an action.

### Common Technologies

Non-repudiation is commonly supported by:

- Digital signatures
- Digital certificates
- Public Key Infrastructure (PKI)

### Security Risks

Shared accounts reduce non-repudiation because individual accountability is lost.

---

## Important Exam Concepts

| Scenario | Best Answer |
|----------|--------------|
| Security policies and training | Managerial Control |
| Daily patching and backups | Operational Control |
| Firewall or IDS | Technical Control |
| Prevent attacks before they occur | Preventive Control |
| Detect suspicious activity | Detective Control |
| Restore systems after incidents | Corrective Control |
| Discourage attacks | Deterrent Control |
| Alternative protection | Compensating Control |
| Define behavior through policy | Directive Control |
| Verify identity | Authentication |
| Determine access rights | Authorization |
| Log user activity | Accounting |
| Prevent denial of actions | Non-Repudiation |

---

## Summary

Security controls help organizations:

- Prevent attacks
- Detect incidents
- Recover from disruptions
- Enforce policies
- Maintain accountability

AAA ensures secure access management, while non-repudiation supports accountability and legal evidence.

---
