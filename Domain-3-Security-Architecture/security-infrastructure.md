# Security Infrastructure

## 1. Security Infrastructure and Enforcement

### 1.1 What is Security Infrastructure?

Security infrastructure refers to the technologies, processes, and policies used to protect an organization's systems, networks, applications, and data.

#### Core Components

##### Hardware

Examples include:

- Firewalls
- Switches
- Routers
- Web Application Firewalls (WAFs)
- Load Balancers
- Network Sensors

##### Software

Examples include:

- Antivirus (AV)
- Endpoint Detection and Response (EDR)
- Data Loss Prevention (DLP)
- Security Information and Event Management (SIEM)
- Host-Based Intrusion Detection Systems (HIDS)
- Security Agents

##### Network Infrastructure

Examples include:

- LAN
- WAN
- VPN
- SD-WAN
- SASE

##### Data Assets

Examples include:

- Databases
- File Servers
- Backups
- Log Repositories

##### Policies and Procedures

Examples include:

- Identity and Access Management (IAM) policies
- Password policies
- Incident response procedures
- Change management processes

#### Security Objectives

- Protect **Confidentiality**
- Protect **Integrity**
- Protect **Availability**
- Reduce risk exposure
- Minimize the attack surface

---

## 2. Firewalls

### 2.1 Basic Concepts

A firewall is a security device or software solution that permits or denies network traffic based on predefined rules.

---

### Screened Subnet (DMZ)

A screened subnet creates a buffer zone between external networks and internal systems.

Typical architecture:

```text
Internet → Firewall → DMZ → Firewall → Internal Network
```

Purpose:

- Isolate public-facing services
- Reduce direct exposure of internal systems

---

## 2.2 Firewall Types

| Type | OSI Layer | Function | Notes |
|------|------------|----------|-------|
| **Packet Filtering Firewall** | Layer 3 / Layer 4 | Filters traffic based on IP, port, and protocol | Fast and simple |
| **Stateful Firewall** | Layer 4 | Tracks connection states | Allows return traffic automatically |
| **Proxy Firewall** | Layer 5 / Layer 7 | Acts as an intermediary between client and server | Hides client identity |
| **Kernel Proxy Firewall** | Full Stack | Performs deep inspection at the kernel level | High performance |

---

## 2.3 NGFW vs UTM vs WAF

### Next-Generation Firewall (NGFW)

Features:

- Application awareness
- Deep Packet Inspection (DPI)
- Integrated IDS and IPS
- User identity integration
- URL filtering

NGFW typically uses a unified inspection engine.

---

### Unified Threat Management (UTM)

UTM combines multiple security functions into a single platform.

Examples:

- Firewall
- IPS
- Antivirus
- URL Filtering

Advantages:

- Easier management
- Reduced device complexity

Risks:

- Single point of failure

---

### Web Application Firewall (WAF)

WAF protects web applications by inspecting HTTP and HTTPS traffic.

Protects against attacks such as:

- SQL Injection
- Cross-Site Scripting (XSS)

Deployment options:

- **Inline** → Blocks malicious traffic
- **Out-of-Band** → Detects and alerts only

---

## 2.4 Layer 4 vs Layer 7 Firewalls

### Layer 4 Firewall

Inspects:

- TCP
- UDP
- Ports

Examples:

- Port 80
- Port 443

---

### Layer 7 Firewall

Inspects:

- HTTP headers
- URLs
- Request methods
- Payload content

---

## 3. ACL and Firewall Rules

### Access Control List (ACL)

ACLs are ordered lists of permit or deny rules.

Key principles:

- First matching rule is applied
- Most devices use an implicit deny rule at the end

Rule components:

- Traffic type
- Source IP and port
- Destination IP and port
- Action (Permit or Deny)

#### Best Practices

- Place specific rules before general rules
- Monitor denied traffic logs regularly

---

## 4. IDS and IPS

### Core Difference

| Technology | Function |
|------------|----------|
| **IDS (Intrusion Detection System)** | Detects and alerts |
| **IPS (Intrusion Prevention System)** | Detects, alerts, and blocks |

---

### IDS Types

#### Network IDS (NIDS)

Monitors network traffic across segments.

#### Host IDS (HIDS)

Monitors a single host or endpoint.

#### Wireless IDS (WIDS)

Detects wireless threats such as rogue access points.

---

### Detection Methods

#### Signature-Based Detection

- Detects known attack patterns
- May miss zero-day attacks

#### Anomaly-Based Detection

- Compares activity to a normal baseline
- Better chance of detecting zero-day attacks
- Higher false positive rate

---

## 5. Network Appliances

### Load Balancer

Distributes traffic across multiple servers.

Benefits:

- Redundancy
- Availability
- Health monitoring

---

### Proxy Server

Acts as an intermediary between users and external resources.

Functions:

- Content caching
- URL filtering
- Authentication
- Data loss prevention

---

### Network Sensors

Used for:

- Traffic monitoring
- Log collection
- Performance metrics

Examples:

- NetFlow sensors
- IDS sensors
- TAP devices

---

### Jump Server

A hardened system used for administrative access to critical systems.

Benefits:

- Centralized logging
- Auditability
- Access control

---

## 6. Port Security and 802.1X

### Port Security

Port security controls which MAC addresses are allowed on switch ports.

#### Common Threat

**MAC Flooding**

An attacker fills the CAM table, forcing the switch to behave like a hub.

#### Security Controls

- Sticky MAC
- Port shutdown
- MAC filtering

---

## 802.1X Authentication

802.1X provides port-based network access control.

### Roles

| Role | Function |
|------|----------|
| **Supplicant** | Client device |
| **Authenticator** | Switch or access point |
| **Authentication Server** | Usually RADIUS |

---

## RADIUS vs TACACS+

| Feature | RADIUS | TACACS+ |
|---------|--------|---------|
| Transport | UDP | TCP |
| Vendor | Open standard | Cisco |
| AAA Separation | Combined | Fully separated |

---

## 7. Secure Network Communications

### VPN Types

#### Site-to-Site VPN

Connects branch offices securely.

#### Client-to-Site VPN

Allows remote users to connect securely.

#### Clientless VPN

Provides secure browser-based access.

---

### Full Tunnel vs Split Tunnel

#### Full Tunnel

- All traffic goes through the VPN
- More secure

#### Split Tunnel

- Only corporate traffic uses VPN
- Better performance

---

## TLS and DTLS

### TLS

Uses TCP.

Common use cases:

- HTTPS
- Email security

### DTLS

Uses UDP.

Common use cases:

- VoIP
- Video streaming

---

## IPSec

Provides:

- Confidentiality
- Integrity
- Authentication
- Anti-Replay Protection

### Modes

#### Transport Mode

- Protects only the payload

#### Tunnel Mode

- Protects the entire packet

---

### IPSec Protocols

| Protocol | Function |
|----------|----------|
| **AH** | Authentication and integrity only |
| **ESP** | Encryption, integrity, and anti-replay |

---

## 8. SD-WAN and SASE

### SD-WAN

Software-defined WAN optimizes traffic across multiple connections.

Examples:

- MPLS
- Broadband
- 4G / 5G

Benefits:

- Centralized management
- Better cloud integration

---

### SASE

Secure Access Service Edge combines networking and security services in the cloud.

Components:

- Firewall as a Service (FWaaS)
- Zero Trust Network Access (ZTNA)
- Cloud Access Security Broker (CASB)
- Secure VPN

Purpose:

- Apply consistent security policies across distributed users

---

## 9. Infrastructure Design Considerations

### Device Placement

Common zones:

- Edge Network
- DMZ
- User Network
- Server Network
- Management Network
- OT / SCADA Networks

Goal:

- Segmentation
- Least trust

---

### Attack Surface Reduction

Reduce exposure by:

- Closing unused ports
- Disabling unnecessary services
- Removing default accounts

---

### Active vs Passive Devices

| Type | Function |
|------|----------|
| **Active** | Interacts with traffic (Firewall, IPS) |
| **Passive** | Monitors traffic only (IDS, TAP) |

---

### Fail-Open vs Fail-Closed

| Mode | Behavior |
|------|----------|
| **Fail-Open** | Traffic continues during failure |
| **Fail-Closed** | Traffic is blocked during failure |

---

## 10. Infrastructure Control Selection

### Core Principles

#### Least Privilege

Users receive only the permissions they need.

#### Defense in Depth

Use multiple layers of security controls.

#### Risk-Based Approach

Focus security investments on critical risks.

#### Lifecycle Management

Continuously review and improve controls.

#### Open Design

Security should depend on strong design principles, not secrecy.

---

## 11. Common Ports and Protocols

| Port | Protocol | Common Use |
|------|----------|------------|
| 21 | FTP | File transfer |
| 22 | SSH, SCP, SFTP | Secure remote access |
| 23 | Telnet | Legacy remote access |
| 25 | SMTP | Email sending |
| 53 | DNS | Name resolution |
| 80 | HTTP | Web traffic |
| 88 | Kerberos | Authentication |
| 110 | POP3 | Email retrieval |
| 143 | IMAP | Email retrieval |
| 161 | SNMP | Device management |
| 389 | LDAP | Directory services |
| 443 | HTTPS | Secure web traffic |
| 445 | SMB | File sharing |
| 636 | LDAPS | Secure directory services |
| 3389 | RDP | Remote desktop |
| 6514 | Syslog over TLS | Secure logging |

---
