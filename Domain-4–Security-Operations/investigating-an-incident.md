# Investigating an Incident

## Incident Investigation

Incident investigation is the process of analyzing security events to understand:

- What happened
- How it happened
- What systems were affected
- What business impact occurred

The goal is to perform an **evidence-based investigation**.

---

## Investigation Data Sources Lifecycle

## 1. Dashboards and Automated Reports

Dashboards and reports often provide the first high-level visibility during an investigation.

### Key Terms

| Term | Description |
|------|-------------|
| **Dashboard** | A visual interface displaying security metrics from multiple systems |
| **Single Pane of Glass** | Centralized visibility of security data in one interface |
| **Automated Report** | Security reports generated automatically by systems |
| **Executive Summary** | A high-level summary for non-technical stakeholders |

### Purpose

- Rapid situational awareness
- Trend analysis
- Incident prioritization

---

## 2. Vulnerability Scans

Vulnerability scans identify known security weaknesses in systems.

### Key Terms

| Term | Description |
|------|-------------|
| **Vulnerability Scan** | Automated scan for known vulnerabilities |
| **False Positive** | A vulnerability reported that does not actually exist |
| **CVE** | Common Vulnerabilities and Exposures identifier |
| **CVSS** | Common Vulnerability Scoring System used to measure severity |

### Important Note

Scan results often require manual validation.

---

## 3. Packet Captures (PCAP)

Packet captures allow investigators to analyze raw network traffic.

### Key Terms

| Term | Description |
|------|-------------|
| **Packet Capture (PCAP)** | Recording of network packets |
| **Source IP** | The originating IP address |
| **Destination IP** | The receiving IP address |
| **Protocol** | Communication protocol such as TCP or UDP |
| **Beaconing** | Repeated communication to the same destination, often malware-related |
| **SYN Flood** | Denial-of-Service attack using repeated TCP SYN requests |

### Goal

- Identify attack behavior
- Analyze communication patterns
- Detect malicious traffic

---

## 4. Security Logs

Logs are one of the most important sources of forensic evidence.

### Common Log Types

| Log Type | Description |
|----------|-------------|
| **Firewall Logs** | Record inbound and outbound traffic |
| **Application Logs** | Record application-level events |
| **Endpoint Logs** | Record user and device activity |
| **Operating System Security Logs** | Record login attempts and privilege changes |
| **IDS Logs** | Detect suspicious activity |
| **IPS Logs** | Detect and automatically block attacks |

---

## 5. SIEM and Event Correlation

### Security Information and Event Management (SIEM)

SIEM collects logs from multiple systems and correlates events.

### Key Concepts

| Concept | Description |
|---------|-------------|
| **Correlation** | Connecting related events across systems |
| **Alert** | Notification triggered by security rules |
| **Trend Analysis** | Detecting abnormal behavior over time |
| **Sensor** | Component that collects logs or telemetry data |

### Purpose

Convert isolated events into meaningful attack scenarios.

---

## 6. Metadata and Evidence

Metadata provides context about data rather than the content itself.

### Key Terms

| Term | Description |
|------|-------------|
| **Metadata** | Data about data |
| **Timestamp** | The date and time of an event |
| **Hash** | Digital fingerprint of a file |
| **Indicator of Compromise (IoC)** | Evidence suggesting system compromise |
| **Chain of Custody** | Documentation of evidence handling |

---

## 7. Automated Response and Analysis

Some security systems automatically respond to detected threats.

### Common Automated Actions

| Action | Description |
|--------|-------------|
| **Account Suspension** | Temporarily disables a user account |
| **IP Blocking** | Blocks malicious IP addresses |
| **Automated Containment** | Isolates affected systems |
| **Incident Analysis** | Evaluates the scope and impact |
| **Root Cause Analysis (RCA)** | Identifies the original cause |

---

## Risk-Based Investigation Perspective

Investigations often include risk analysis.

### Key Risk Concepts

| Concept | Description |
|---------|-------------|
| **Likelihood** | Probability of the event occurring |
| **Impact** | Business effect of the event |
| **Residual Risk** | Remaining risk after controls are applied |
| **Control Effectiveness** | How well security controls perform |

---

## Important Exam Tips

| Scenario | Best Source |
|----------|-------------|
| Overview or trend analysis | SIEM or Dashboard |
| Known vulnerabilities | Vulnerability Scan |
| Raw network traffic | Packet Capture |
| User activity investigation | Endpoint or OS Logs |
| Email investigation | Email Metadata |

---

## Summary

| Data Source | Primary Purpose |
|-------------|-----------------|
| **Dashboards** | High-level visibility |
| **Logs** | Evidence collection |
| **PCAP** | Network traffic analysis |
| **SIEM** | Correlation and alerting |
| **Metadata** | Context and validation |

---

## Important Note

Incident investigations should never rely on a single data source.

Accurate conclusions require correlation across multiple evidence sources.

---
