# Fundamentals of Security

Security fundamentals provide the foundation for understanding how organizations protect data, systems, users, and business operations.

---

## 1. Information Security vs. Information Systems Security

### Information Security

Information security focuses on protecting **data** from unauthorized access, modification, disruption, disclosure, or destruction.

Main focus:

- Data confidentiality
- Data integrity
- Data availability
- Privacy and compliance

### Information Systems Security

Information systems security focuses on protecting the **systems and infrastructure** that store, process, and transmit data.

Examples:

- Servers
- Workstations
- Network devices
- Applications
- Cloud systems

### Key Difference

| Concept | Main Focus |
|---|---|
| Information Security | Data |
| Information Systems Security | Systems and infrastructure |

---

## 2. CIA Triad

The CIA Triad is one of the most important concepts in cybersecurity.

It consists of:

- Confidentiality
- Integrity
- Availability

---

## Confidentiality

Confidentiality ensures that information is only accessible to authorized individuals, systems, or processes.

### Goals

- Protect privacy
- Prevent unauthorized disclosure
- Maintain business advantage
- Support regulatory compliance

### Common Controls

- Encryption
- Access controls
- Data masking
- Physical security
- Security awareness training

### Security+ Exam Tip

If sensitive data is exposed to unauthorized users, it is a **confidentiality violation**.

---

## Integrity

Integrity ensures that data remains accurate, complete, and unaltered unless modified by authorized parties.

### Common Controls

- Hashing
- Digital signatures
- Checksums
- Access controls
- Regular audits

### Important Note

A digital signature provides:

- Integrity
- Authenticity
- Non-repudiation

### Security+ Exam Tip

If data is modified without authorization, it is an **integrity violation**.

---

## Availability

Availability ensures that systems, services, and data are accessible when needed.

### Why Availability Matters

- Business continuity
- Customer trust
- Operational stability
- Organizational reputation

### Common Controls

- Redundant servers
- Data backups
- Network redundancy
- Power redundancy
- Disaster recovery planning
- DDoS protection

### Security+ Exam Tip

If a system is unavailable due to outage, failure, or denial-of-service, it is an **availability violation**.

---

## 3. Non-Repudiation

Non-repudiation ensures that a user cannot deny performing an action.

It is commonly achieved through **digital signatures**.

### Digital Signature Process

1. A message is hashed.
2. The hash is encrypted with the sender's private key.
3. The recipient verifies the signature using the sender's public key.

### Provides

- Authenticity
- Integrity
- Non-repudiation

---

## 4. AAA Framework

AAA stands for:

- Authentication
- Authorization
- Accounting

---

## Authentication

Authentication verifies identity.

In simple terms:

> Are you really who you claim to be?

### Authentication Factors

| Factor | Example |
|---|---|
| Something you know | Password, PIN |
| Something you have | Token, smart card |
| Something you are | Fingerprint, facial recognition |
| Something you do | Typing pattern, behavior |
| Somewhere you are | Location-based authentication |

### Multi-Factor Authentication

MFA uses two or more different authentication factors.

### Security+ Exam Tip

Authentication is about **identity verification**.

---

## Authorization

Authorization determines what an authenticated user is allowed to do.

Examples:

- Read-only access
- Write permission
- Administrator privileges
- Role-based access

### Security+ Exam Tip

Authorization is about **permissions**.

---

## Accounting

Accounting tracks user activity and system events.

### Purpose

- Audit trails
- Forensic analysis
- Compliance
- User accountability

### Common Technologies

- Syslog servers
- SIEM systems
- Network monitoring tools
- Audit logs

---

## 5. Security Controls

Security controls are safeguards used to reduce risk and protect assets.

---

## Security Control Categories

| Category | Description | Examples |
|---|---|---|
| Technical | Implemented using technology | Firewalls, IDS/IPS, encryption |
| Managerial | Administrative and governance-focused | Policies, risk assessments, governance |
| Operational | People and process-based | Procedures, training, incident response |
| Physical | Protect physical assets | Locks, cameras, guards |

---

## Security Control Types

| Type | Purpose | Example |
|---|---|---|
| Preventive | Stops an incident before it happens | Firewall, access control |
| Deterrent | Discourages an attacker | Warning banner, security guard |
| Detective | Identifies an incident | IDS, logs, SIEM alerts |
| Corrective | Restores or fixes after an incident | Patching, backups |
| Compensating | Alternative control when primary control is not possible | Manual review instead of automated control |
| Directive | Guides behavior through rules or instructions | Policies, procedures |

### Security+ Exam Tip

Security control questions are often scenario-based. Focus on what the control is trying to achieve.

---

## 6. Threat, Vulnerability, and Risk

### Threat

A threat is anything that has the potential to cause harm.

Examples:

- Malware
- Insider threat
- Natural disaster
- Cybercriminal group

### Vulnerability

A vulnerability is a weakness that can be exploited by a threat.

Examples:

- Unpatched software
- Weak passwords
- Misconfigured firewall
- Lack of security awareness

### Risk

Risk exists when a threat can exploit a vulnerability.

A simple way to remember:

```text
Risk = Threat + Vulnerability
```

### Key Logic

| Situation | Risk? |
|---|---|
| Threat exists, but no vulnerability | Low or no risk |
| Vulnerability exists, but no relevant threat | Low or no risk |
| Threat and vulnerability both exist | Risk exists |

This is the core logic behind vulnerability management.

---

## 7. Risk Management

Risk management is the process of identifying, assessing, prioritizing, and reducing risk.

### Main Goals

- Reduce likelihood
- Reduce impact
- Support business objectives
- Achieve the desired security outcome

In cybersecurity, security decisions are often risk management decisions.

---

## 8. Gap Analysis

Gap analysis identifies the difference between the current state and the desired future state.

### Steps

1. Define the scope.
2. Analyze the current state.
3. Identify gaps.
4. Create an action plan.

### Types

- Technical gap analysis
- Business gap analysis

### Output: POA&M

POA&M stands for **Plan of Action and Milestones**.

It usually includes:

- Identified vulnerabilities
- Required remediation actions
- Timeline
- Responsible teams
- Required resources

---

## 9. Zero Trust

Zero Trust is a security model based on the principle:

> Never trust, always verify.

Being inside the network does not automatically mean a user or device should be trusted.

---

## Control Plane

The control plane is responsible for policy decisions and access logic.

It includes:

- Adaptive identity
- Threat scope reduction
- Policy-driven access
- Secured zones
- Policy engine
- Policy administrator

### Security+ Exam Tip

The control plane decides whether access should be allowed.

---

## Data Plane

The data plane is where access is actually enforced.

It includes:

- Subject
- Policy Enforcement Point (PEP)

### Security+ Exam Tip

The data plane enforces access decisions.

---

## Key Security+ Takeaways

- The CIA Triad is the foundation of security.
- Confidentiality protects data from unauthorized disclosure.
- Integrity protects data from unauthorized modification.
- Availability ensures systems and data are accessible when needed.
- Authentication verifies identity.
- Authorization determines permissions.
- Accounting tracks activity.
- Digital signatures provide integrity, authenticity, and non-repudiation.
- Risk exists when a threat can exploit a vulnerability.
- Zero Trust requires continuous verification.
