# Alerting and Monitoring

Alerting and monitoring are essential for protecting the core principles of information security:

- **Confidentiality**
- **Integrity**
- **Availability**

These processes help organizations detect threats early, respond quickly, and reduce operational risk.

---

## Alerting vs Monitoring

### Monitoring

Monitoring is the continuous observation of systems, networks, and security events.

### Key Objectives

- Detect anomalies
- Identify performance degradation
- Discover security threats
- Support proactive security operations

---

### Alerting

Alerting generates notifications when predefined conditions are met.

### Common Alert Delivery Methods

- Email
- SMS
- Dashboards
- Ticketing systems

### Key Objective

Enable security teams to take immediate action.

---

## Alert Classifications

| Alert Type | Description |
|------------|-------------|
| **True Positive** | A real threat is correctly identified |
| **False Positive** | An alert is generated when no threat exists |
| **True Negative** | Normal activity is correctly identified |
| **False Negative** | A real threat is missed |

---

## Alerting Goals

Security teams aim to:

- Increase true positives
- Reduce false positives
- Prevent alert fatigue

---

## Monitoring Types

### Automated Monitoring

Automated monitoring uses software-based systems.

### Benefits

- Continuous monitoring
- Scalable for large environments
- Real-time detection

---

### Manual Monitoring

Manual monitoring relies on human analysis.

### Activities

- Log review
- Incident investigation
- Security analysis

### Benefits

Provides deeper contextual understanding.

---

## System Monitoring

Organizations commonly monitor:

- CPU utilization
- Memory usage
- Disk utilization
- Network performance

---

## Baseline Monitoring

A baseline represents normal system behavior.

Examples include:

- Normal CPU usage
- Normal RAM consumption
- Normal network traffic

### Purpose

Identify abnormal behavior by comparing current activity to expected patterns.

---

## Monitoring Activities

## Log Aggregation

Log aggregation centralizes logs from multiple systems.

### Benefits

- Simplifies analysis
- Supports event correlation
- Supports incident investigation
- Supports compliance requirements

---

## Alerting Mechanisms

Alerts may be triggered by:

- Threshold violations
- Behavioral anomalies
- Known attack signatures

---

## Security Scanning

Scanning identifies vulnerabilities and security weaknesses.

### Common Scanning Types

| Scan Type | Purpose |
|-----------|---------|
| **Vulnerability Scanning** | Identifies known vulnerabilities |
| **Configuration Scanning** | Detects misconfigurations |
| **Code Scanning** | Identifies software security flaws |

---

## Reporting

Security reports are created from collected monitoring data.

### Common Uses

- Performance analysis
- Security posture reviews
- Compliance reporting
- Continuous improvement

---

## Archiving

Archiving stores logs and security records for long-term retention.

### Common Purposes

- Regulatory compliance
- Forensic investigations
- Historical analysis

Cloud storage is commonly used for archival purposes.

---

## Alert Response and Remediation

### Alert Response

Response activities include:

- Alert validation
- Escalation
- Incident response activation

---

### Remediation

Remediation may include:

- Applying security patches
- Correcting configurations
- Removing vulnerabilities

---

### Validation

Validation confirms whether remediation actions were successful.

---

### Quarantining

Quarantining isolates suspicious systems to prevent threat propagation.

Examples:

- Malware containment
- Endpoint isolation

---

## Alert Tuning

Alert tuning optimizes detection rules and thresholds.

### Benefits

- Reduces false positives
- Improves SOC efficiency
- Improves detection quality

---

## SNMP (Simple Network Management Protocol)

SNMP is used to monitor network devices.

Examples:

- Routers
- Switches
- Firewalls
- Servers

---

## SNMP Components

| Component | Description |
|-----------|-------------|
| **SNMP Manager** | Central monitoring system |
| **SNMP Agent** | Software running on monitored devices |

---

## SNMP Message Types

| Message Type | Function |
|--------------|----------|
| **GET** | Requests information |
| **SET** | Modifies a configuration value |
| **TRAP** | Sends automatic event notifications |

---

## SNMP Version 3 Security

SNMPv3 provides:

- Authentication
- Integrity
- Confidentiality through encryption

---

## SIEM (Security Information and Event Management)

SIEM centralizes log and event data from multiple sources.

### Core Functions

- Log collection
- Event correlation
- Threat detection
- Behavioral analysis

---

## Agent-Based vs Agentless Monitoring

| Type | Description |
|------|-------------|
| **Agent-Based** | Provides detailed real-time data |
| **Agentless** | Easier maintenance with less detail |

---

## Common SIEM Platforms

Examples include:

- Splunk
- ELK Stack
- IBM QRadar
- ArcSight

---

## Common SIEM Data Sources

SIEM platforms often collect data from:

- Antivirus solutions
- Data Loss Prevention systems
- NIDS and NIPS
- Firewalls
- Vulnerability scanners

---

## SCAP (Security Content Automation Protocol)

SCAP is a framework for automated vulnerability management.

It was developed by **NIST**.

---

## SCAP Components

| Component | Description |
|-----------|-------------|
| **OVAL** | Open Vulnerability and Assessment Language |
| **XCCDF** | Security configuration benchmark definitions |
| **ARF** | Asset Reporting Format |

---

## Security Enumeration Standards

| Standard | Purpose |
|----------|---------|
| **CVE** | Vulnerability identification |
| **CPE** | Platform enumeration |
| **CCE** | Configuration issue identification |
| **CVSS** | Vulnerability severity scoring |

---

## Network Flow Analysis

Flow analysis focuses on network metadata instead of full packet contents.

### Benefits

- Detect traffic anomalies
- Identify suspicious communication patterns
- Detect traffic spikes

---

## NetFlow and IPFIX

Used for:

- Traffic analysis
- Performance monitoring
- Security visibility

---

## Zeek

Zeek provides advanced network analysis.

### Capabilities

- Flow analysis
- Protocol analysis
- Packet inspection
- Threat detection

---

## Single Pane of Glass (SPOG)

Single Pane of Glass centralizes security visibility into one interface.

### Benefits

- Faster decision-making
- Improved operational efficiency
- Better incident correlation

---

## Summary

Alerting and monitoring provide:

- Proactive threat detection
- Faster incident response
- Operational visibility
- Improved SOC efficiency

---
