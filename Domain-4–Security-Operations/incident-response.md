# Incident Response

Incident Response (IR) is a structured process used to identify, contain, eradicate, and recover from security incidents.

The goal is to restore systems securely while minimizing operational impact.

---

## Incident Response Objectives

The primary objectives of incident response include:

- Minimizing operational impact
- Reducing detection and containment time
- Maintaining business continuity
- Supporting secure recovery
- Preventing future incidents

---

## Core Incident Response Activities

Incident response typically includes:

- Detection
- Classification
- Containment
- Eradication
- Recovery
- Evidence Preservation
- Communication
- Lessons Learned

---

## Incident Response Lifecycle

CompTIA uses an expanded **7-phase incident response model**.

---

## 1. Preparation

Preparation occurs before an incident takes place.

### Key Activities

- Develop policies and procedures
- Create incident response plans
- Harden systems
- Define communication channels
- Assign the Incident Response Team (IRT)

### Goal

Ensure the organization is ready before an incident occurs.

---

## 2. Detection

Detection identifies whether a security incident is occurring.

### Common Detection Tools

Examples include:

- SIEM
- IDS
- IPS
- EDR
- Security Logs

### Goal

Determine whether suspicious or malicious activity exists.

---

## 3. Analysis

Analysis determines the scope, severity, and business impact of the incident.

### Key Questions

- Which systems are affected?
- What is the attack vector?
- How severe is the incident?
- What business services are impacted?

### Additional Actions

- Notify stakeholders
- Begin incident classification

---

## 4. Containment

Containment prevents the incident from spreading.

### Common Actions

- Isolate compromised systems
- Disable affected accounts
- Block malicious IP addresses
- Restrict network access

### Goal

Limit damage while preserving business operations.

---

## 5. Eradication

Eradication removes the root cause of the incident.

### Common Actions

- Remove malware
- Eliminate backdoors
- Remove persistence mechanisms
- Patch vulnerabilities
- Reimage compromised systems if necessary

### Important Note

Eradication begins after containment.

---

## 6. Recovery

Recovery restores systems to normal business operations.

### Common Actions

- Restore systems from backups
- Validate system integrity
- Apply security patches
- Verify configurations
- Monitor for recurring activity

### Goal

Return to secure normal operations.

---

## 7. Post-Incident Activity

Post-incident activities improve future incident response.

### Common Activities

- Root Cause Analysis (RCA)
- Lessons Learned meetings
- After-Action Reports
- Security control improvements
- Incident response plan updates

---

## Root Cause Analysis (RCA)

Root Cause Analysis identifies why an incident occurred.

### Goals

- Identify the original cause
- Prevent recurrence
- Improve security processes

### RCA Process

1. Define the incident
2. Analyze causal relationships
3. Identify corrective actions
4. Implement and monitor improvements

---

## No-Blame Culture

Effective incident response focuses on:

- Process improvement
- Honest reporting
- Organizational learning

The goal is not to blame individuals.

---

## Threat Hunting

Threat hunting is a proactive security activity.

Instead of waiting for alerts, analysts actively search for hidden threats.

---

## Threat Hunting Goals

- Detect hidden threats
- Discover previously unknown attacks
- Identify new attacker TTPs (Tactics, Techniques, and Procedures)

---

## Threat Hunting Process

### 1. Hypothesis Development

Assume compromise may already exist.

### 2. Threat Actor Profiling

Study attacker behavior patterns.

### 3. Data Analysis

Analyze:

- Logs
- System activity
- Registry entries
- Network traffic

### 4. Discovery

Identify new attack techniques or hidden compromises.

---

## Incident Response Team (IRT)

The Incident Response Team manages security incidents.

### Common Roles

| Role | Responsibility |
|------|----------------|
| **Team Leader** | Coordinates the incident response process |
| **Subject Matter Experts (SMEs)** | Provide technical expertise |
| **IT Support** | Supports infrastructure recovery |
| **Legal Counsel** | Handles legal obligations |
| **Human Resources** | Manages employee-related incidents |
| **Public Relations** | Handles external communications |

---

## Incident Response Training and Testing

Regular training improves response readiness.

### Training Types

- Role-based training
- Security awareness training
- Lessons learned reviews

---

## Testing Methods

| Test Type | Description |
|-----------|-------------|
| **Tabletop Exercise (TTX)** | Scenario-based team discussions |
| **Simulation** | Simulated cyber incidents |
| **Drills** | Practice specific procedures |
| **Live Exercises** | Realistic operational testing |
| **Penetration Testing** | Controlled offensive security testing |

---

## Digital Forensics

Digital forensics supports incident investigation and legal proceedings.

### Objectives

- Collect evidence
- Support investigations
- Identify attack methods
- Support legal action

---

## Digital Forensics Phases

### 1. Identification

Identify evidence sources and secure the scene.

---

### 2. Collection

Collect evidence using approved forensic procedures.

### Important Principle

Follow the **Order of Volatility**.

---

### 3. Analysis

Analyze forensic images instead of original systems.

Examples:

- Timestamps
- User activity
- File changes
- Malware artifacts

---

### 4. Reporting

Document findings in a formal report.

Reports may be used in legal proceedings.

---

## Order of Volatility

Always collect the most volatile evidence first.

### Collection Priority

1. CPU Registers and Cache
2. RAM and Running Processes
3. Disk and Persistent Storage
4. Network Logs
5. Physical Configuration
6. Archived Data

### Important Exam Tip

RAM is always collected before disk data.

---

## Evidence Collection Techniques

Common forensic collection methods include:

- Disk imaging
- File carving
- Hash verification
- Screenshots
- Network log collection
- CCTV recordings

---

## Legal Concepts

### Chain of Custody

Documents:

- Who handled evidence
- When it was handled
- How it was stored

---

### Legal Hold

Preserves data when legal action is expected.

---

### E-Discovery

The process of collecting electronic evidence for legal investigations.

---

## Data Acquisition

Data acquisition creates a forensically sound copy of evidence.

### Important Considerations

- Never analyze the original disk directly
- BYOD environments may introduce legal complications
- Some evidence exists only in volatile memory

---

## Important Exam Notes

- **Order of Volatility** → RAM is collected before disk
- **Recovery ≠ Eradication**
- **Threat Hunting = Proactive**
- **RCA focuses on improvement, not blame**
- **Forensic analysis should never be performed on original evidence**

---
