# System Hardening

## Overview

Hardening is the process of making systems, applications, and networks more resistant to cyberattacks.

The main objectives are:

- Reduce the attack surface
- Improve security posture
- Maintain the CIA Triad:
  - Confidentiality
  - Integrity
  - Availability

In Security+, hardening is closely related to:

- Mitigation techniques
- System and resource security
- Enterprise security enhancement

---

## What is Hardening?

Hardening removes insecure default configurations and unnecessary services to improve system security.

### Common Hardening Actions

- Apply security patches
- Change default passwords
- Disable unnecessary services and ports
- Configure access controls
- Establish secure baselines

### Primary Goal

Strengthen overall security posture and improve resilience against cyber threats.

---

## Default Configurations

Default configurations are commonly targeted by attackers.

---

## Default Passwords

Default credentials should:

- Be changed immediately after installation
- Be rotated regularly
- Be managed securely

### Best Practices

- Use strong passwords
- Rotate passwords periodically
- Use password managers

---

## Default Ports and Protocols

Unnecessary ports and insecure protocols should be disabled.

### Best Practices

- Close unused ports
- Perform regular audits
- Replace insecure protocols with secure alternatives

### Examples

| Insecure Protocol | Secure Alternative |
|-------------------|-------------------|
| **Telnet** | **SSH** |
| **HTTP** | **HTTPS** |
| **FTP** | **SFTP** |

---

## Least Functionality

The **Least Functionality Principle** states that systems should run only the applications and services required for business operations.

### Security Benefits

- Reduces attack surface
- Improves performance
- Simplifies security management

### Common Actions

- Remove unused software
- Disable unnecessary services
- Restrict unauthorized applications

---

## Application Control

Application control limits which software can execute.

---

## Application Allowlisting

Only approved applications are allowed to run.

### Characteristics

- Default action = Deny
- Higher security
- More administrative effort

---

## Application Blocklisting

Only explicitly blocked applications are denied.

### Characteristics

- Default action = Allow
- Easier to manage
- Less secure

---

## Important Exam Note

**Allowlisting provides stronger security than blocklisting.**

---

## Secure Baseline Images

A secure baseline is a trusted configuration used when deploying new systems.

### Typical Baseline Components

- Updated operating system
- Minimum required applications
- Secure configurations
- Security agents such as antivirus or EDR

### Best Practice

Baselines should be reviewed and updated regularly.

---

## Trusted Operating Systems (TOS)

Trusted operating systems enforce security policies at the system level.

### Core Features

- Mandatory Access Control (MAC)
- Security auditing
- Role-Based Access Control (RBAC)

---

## Evaluation Assurance Levels (EAL)

EAL measures the assurance level of a trusted system under **Common Criteria**.

| Level | Meaning |
|-------|---------|
| **EAL 1** | Basic assurance |
| **EAL 7** | Highest assurance |

---

## Common Examples

Examples of trusted operating systems:

- SELinux
- Trusted Solaris

---

## Updates and Patches

Regular patching is critical for system security.

---

## Patch Types

### Hotfix

Emergency fix for critical vulnerabilities.

### Update

General improvements or feature changes.

### Service Pack

A bundled collection of updates and fixes.

---

## Important Security Consideration

Attackers may reverse-engineer patches to identify vulnerabilities in unpatched systems.

---

## Patch Management

Patch management is the process of:

- Planning
- Testing
- Deploying
- Auditing patches

---

## Patch Management Lifecycle

### 1. Planning

Identify systems and patch requirements.

### 2. Testing

Test patches in controlled environments.

### 3. Implementation

Deploy patches to production systems.

### 4. Auditing

Verify successful deployment.

---

## Enterprise Patch Management

Large environments often use:

- Central update servers
- Patch rings
- Mobile Device Management (MDM)

---

## Group Policy (Windows)

Group Policy Objects (GPOs) enforce security settings across Windows environments.

### Common Use Cases

- Password policies
- Account lockout policies
- Software restrictions
- Security settings

---

## AppLocker

AppLocker provides application control in Windows.

### Rule Types

- Publisher-based rules
- Path-based rules
- Hash-based rules

### Purpose

Enforce application allowlisting and support secure baselines.

---

## SELinux (Security-Enhanced Linux)

SELinux is a Linux security framework that implements **Mandatory Access Control (MAC)**.

It was originally developed by the **NSA**.

---

## DAC vs MAC

| Access Model | Description |
|--------------|-------------|
| **DAC (Discretionary Access Control)** | Users control access permissions |
| **MAC (Mandatory Access Control)** | The system enforces access policies |

---

## SELinux Modes

| Mode | Description |
|------|-------------|
| **Disabled** | SELinux is turned off |
| **Permissive** | Logs policy violations without enforcement |
| **Enforcing** | Actively enforces security policies |

---

## SELinux Context Types

SELinux labels may include:

- User
- Role
- Type
- Level (optional)

---

## Logging

SELinux events are typically recorded in audit logs.

---

## Data Encryption Levels

Encryption can be applied at multiple levels.

### Common Types

- Full Disk Encryption
- Partition Encryption
- Volume Encryption
- File-Level Encryption
- Database Encryption
- Record-Level Encryption

---

## Important Concept

More granular encryption provides greater control but increases management complexity.

---

## Secure Baselines

A secure baseline defines the minimum accepted security configuration.

### Common References

Organizations often use:

- :contentReference[oaicite:1]{index=1}
- :contentReference[oaicite:2]{index=2}

---

## Secure Baseline Lifecycle

### 1. Assessment

Evaluate the current environment.

### 2. Configuration

Apply secure settings.

### 3. Deployment

Deploy to production systems.

### 4. Monitoring

Track compliance and deviations.

### 5. Maintenance

Review and update configurations regularly.

---

## Primary Goals

- Consistency
- Visibility
- Control

---

## User Awareness

Security also depends on user behavior.

Users should be trained to:

- Understand secure baselines
- Avoid unauthorized software
- Report suspicious activity

---

## Important Exam Tips

- Allowlisting is more secure than blocklisting
- MAC is different from DAC
- Hotfixes usually address critical security issues
- Updates are not always security patches
- Baseline means a known good configuration

---
