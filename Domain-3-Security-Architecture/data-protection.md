# Data Protection

## Overview

Data protection is the process of safeguarding data against:

- Corruption
- Unauthorized access
- Loss

The primary goal is to maintain:

- **Confidentiality**
- **Integrity**
- **Availability**

---

## Data Classification

Data classification is the process of categorizing data based on its value, sensitivity, and business impact.

This helps organizations apply appropriate security controls.

### Common Data Classification Types

- Sensitive
- Confidential
- Public
- Restricted
- Private
- Critical

---

## Commercial Business Classification Levels

| Level | Description |
|-------|-------------|
| **Public** | Information that can be shared openly without risk |
| **Sensitive** | Information that may cause minor impact if disclosed |
| **Private** | Personal or employee-related information |
| **Confidential** | Trade secrets, source code, or intellectual property |
| **Critical** | Mission-critical business data requiring the highest protection |

---

## Government Classification Levels

| Level | Description |
|-------|-------------|
| **Unclassified** | Publicly available information |
| **Sensitive but Unclassified** | Moderately sensitive operational or personal information |
| **Confidential** | Information that may impact government operations if disclosed |
| **Secret** | Military or strategic defense information |
| **Top Secret** | Information that could cause severe national security damage if exposed |

---

## Importance of Data Classification

Proper classification helps organizations:

- Allocate security resources effectively
- Avoid overclassification and unnecessary costs
- Improve data governance and protection

---

## Data Ownership Roles

| Role | Responsibility |
|------|----------------|
| **Data Owner** | Responsible for data confidentiality, integrity, and availability |
| **Data Controller** | Determines how and why data is collected, processed, and stored |
| **Data Processor** | Processes data on behalf of the data controller |
| **Data Steward** | Maintains data quality, labeling, and consistency |
| **Data Custodian** | Manages technical storage, access control, and backups |
| **Privacy Officer** | Ensures compliance for sensitive personal or health-related data |

### Important Note

Business units usually own the data.

IT departments are typically responsible for:

- Technical protection
- Access management
- Backup operations

---

## Data States

### Data at Rest

Stored data located on:

- Hard drives
- SSDs
- Databases
- Backup systems

#### Protection Methods

- Full Disk Encryption (FDE)
- File Encryption
- Database Encryption

---

### Data in Transit

Data actively moving across networks.

#### Protection Methods

- TLS / SSL
- VPN
- IPSec

---

### Data in Use

Data actively being processed by applications or systems.

#### Protection Methods

- Application-level encryption
- Access controls
- Secure enclaves

---

## Data Types

| Type | Description |
|------|-------------|
| **Regulated Data** | Data governed by regulations such as GDPR or HIPAA |
| **PII (Personally Identifiable Information)** | Information that can identify an individual |
| **PHI (Protected Health Information)** | Health-related personal information |
| **Trade Secrets** | Proprietary business processes or confidential strategies |
| **Intellectual Property (IP)** | Patents, copyrights, source code, or designs |
| **Legal Information** | Contracts, litigation records, or regulatory documentation |
| **Financial Information** | Banking records, tax documents, or financial statements |
| **Human-Readable Data** | Information readable by humans, such as text |
| **Machine-Readable Data** | Information processed by systems, such as binary data |

---

## Data Sovereignty

Data sovereignty means that data is subject to the laws of the country where it is stored.

Examples include:

### European Union

- **GDPR**
- Restricts data processing outside approved regions

### United States

Examples:

- HIPAA
- CCPA

### Other Countries

Some countries require data localization, meaning data must remain within national borders.

### Cloud Security Consideration

Cloud environments may store data in multiple regions, creating regulatory compliance challenges.

---

## Data Security Methods

| Method | Description |
|--------|-------------|
| **Encryption** | Protects data confidentiality |
| **Hashing** | Ensures data integrity |
| **Masking** | Hides sensitive portions of data |
| **Tokenization** | Replaces sensitive data with non-sensitive tokens |
| **Obfuscation** | Makes data intentionally difficult to understand |
| **Segmentation** | Limits the spread of attacks by isolating systems |
| **Geofencing** | Restricts access based on geographic location |
| **Permission Restriction** | Uses access controls such as ACL or RBAC |

---

## Data Loss Prevention (DLP)

Data Loss Prevention (DLP) is a strategy used to prevent sensitive data from leaving the organization.

DLP systems monitor data in three states:

- **Data in Use**
- **Data in Transit**
- **Data at Rest**

---

## Types of DLP Solutions

| Type | Description |
|------|-------------|
| **Endpoint DLP** | Monitors data activity on user devices |
| **Network DLP** | Inspects network traffic for data leakage |
| **Storage DLP** | Monitors stored data in servers and data centers |
| **Cloud-Based DLP** | Protects sensitive data in cloud platforms |

---

## Summary

| Topic | Key Concept |
|-------|-------------|
| **Data Classification** | Categorizing data based on sensitivity |
| **Data Ownership** | Defining roles and responsibilities |
| **Data States** | Protecting data at rest, in transit, and in use |
| **Data Sovereignty** | Following regional data regulations |
| **Data Security Methods** | Encryption, hashing, masking, tokenization |
| **DLP** | Preventing unauthorized data leakage |

---
