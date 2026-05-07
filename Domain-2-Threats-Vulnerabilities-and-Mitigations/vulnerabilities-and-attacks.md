# Vulnerabilities and Attacks  

## 1. Overview – Vulnerabilities vs. Attacks

### 1.1 What is a Vulnerability?

- **Definition:**  
  Weaknesses found in hardware, software, configurations, or operational processes.
  
- **Potential Impact:**
  - Unauthorized access
  - Data breaches
  - Service disruption or system failure

### 1.2 What is an Attack?

- **Definition:**  
  A deliberate action performed by a threat actor to exploit a vulnerability.

- **Common Objectives:**
  - Unauthorized access
  - Data theft
  - Malware delivery
  - DoS / DDoS attacks
  - Social engineering

---

## 2. Hardware Vulnerabilities

### 2.1 Definition

> Security weaknesses caused by hardware components, firmware, or physical design flaws.

### 2.2 Types of Hardware Vulnerabilities

#### 2.2.1 Firmware Vulnerabilities

- Firmware = Embedded software running directly on hardware.
- Risks:
  - Outdated or unpatched firmware
  - Insecure development practices
  - Unsigned firmware updates
  - If exploited, attackers may gain full administrative or root access

#### 2.2.2 End-of-Life (EOL), Legacy, and Unsupported Systems

- **End-of-Life (EOL):** Systems no longer supported by the vendor.
- **Legacy Systems:** Older technologies still in use despite newer alternatives.
- **Unsupported Systems:** No official support, patches, or security updates.

- **Security Risk:**  
  Known vulnerabilities remain unpatched, making them easy targets.

#### 2.2.3 Unpatched Systems

- Systems missing the latest security updates.

- Common causes:
  - Negligence
  - Operational complexity
  - Fear of downtime

- Security Risk:
  - Publicly documented vulnerabilities
  - Widely available exploit code

#### 2.2.4 Hardware Misconfigurations

- Improper or default configurations:
  - Default passwords
  - Unnecessary open services or ports
  - Incorrect ACLs
  - Misconfigured VLANs

- Common causes:
  - Rushed deployments
  - Poor documentation
  - Lack of expertise

### 2.3 Mitigations for Hardware Vulnerabilities

- **Hardening**
  - Disable unnecessary ports and services
  - Enforce strong passwords and MFA
  - Change or disable default accounts

- **Patching**
  - Regularly update firmware, operating systems, and applications

- **Configuration Enforcement**
  - Apply secure baseline configurations automatically (GPO, Ansible, etc.)

- **Decommissioning**
  - Retire EOL or legacy systems in a planned manner

- **Isolation & Segmentation**
  - Place older or vulnerable systems in separate VLANs or network segments
  - Allow only necessary traffic through firewall rules or ACLs

---

## 3. Bluetooth Vulnerabilities and Attacks

### 3.1 Bluetooth Overview

- A short-range wireless communication technology.

- Security Risks:
  - Insecure pairing
  - Device spoofing
  - On-path (Man-in-the-Middle) attacks

### 3.2 Common Bluetooth Attacks

| Attack | Description |
|--------|-------------|
| **Bluejacking** | Sending unsolicited messages to nearby devices |
| **Bluesnarfing** | Unauthorized access to device data such as contacts, SMS, or call logs |
| **Bluebugging** | Gaining control over Bluetooth functions such as calls, messages, or internet access |
| **Bluesmack** | Flooding attack causing denial of service |
| **BlueBorne** | Airborne attack family enabling remote code execution without user interaction |

### 3.3 Bluetooth Security Best Practices

- Turn Bluetooth off when not in use
- Keep devices in **non-discoverable mode**
- Pair only with trusted devices
- Use unique PINs or passkeys
- Keep firmware updated
- Reject suspicious connection requests
- Use encryption for sensitive data transmission

---

## 4. Mobile Vulnerabilities and Attacks

### 4.1 Sideloading

- **Definition:**  
  Installing applications from third-party sources instead of official app stores.

- **Risks:**
  - Malware
  - Trojans
  - Spyware

- **Mitigation:**
  - Keep unknown sources disabled
  - Install apps only from official or enterprise app stores

### 4.2 Jailbreaking / Rooting

- **Purpose:**  
  Gaining administrative or root privileges on mobile devices.

- **Risks:**
  - Disables built-in security controls
  - Can prevent official updates
  - Malicious applications may gain elevated privileges

### 4.3 Insecure Connection Methods

- Risks associated with:
  - Public Wi-Fi
  - Open hotspots
  - Unknown Bluetooth devices

- Possible attacks:
  - On-path attacks
  - Packet sniffing
  - ARP spoofing

- **Mitigation:**
  - Use cellular networks or VPN whenever possible
  - Connect only to trusted networks
  - Use strong passwords
  - Implement strong authentication such as 802.1X

### 4.4 Mobile Device Management (MDM)

MDM allows organizations to enforce:

- Regular patching
- Secure configuration management
- Security best practices such as:
  - Blocking sideloading
  - Detecting rooted or jailbroken devices
  - Enforcing VPN, passwords, and screen locks

---

## 5. Zero-Day Vulnerabilities

### 5.1 Key Concepts

- **Zero-Day Vulnerability:**  
  A vulnerability that is newly discovered or unknown to the vendor.

- **Zero-Day Exploit:**  
  Code or technique designed to exploit a zero-day vulnerability.

- **Zero-Day Malware:**  
  Malware that takes advantage of zero-day vulnerabilities.

### 5.2 Why Are Zero-Days Important?

- No patch exists yet
- Difficult to defend against
- Highly valuable in:
  - Bug bounty programs
  - Government intelligence operations
  - Cybercriminal campaigns

### 5.3 Defense Strategies

- Use updated antivirus and EDR solutions
- Deploy IPS / HIPS solutions
- Apply patches immediately once available

---

## 6. Operating System Vulnerabilities

### 6.1 Unpatched Systems

- Missing patches expose systems to known CVEs.

- **Mitigation:**
  - Automatic updates
  - Structured patch management

### 6.2 Zero-Day Vulnerabilities

- Unknown vulnerabilities at the operating system level.

- **Defense:**
  - EDR / HIPS
  - Sandboxing
  - Behavioral analysis
  - Network segmentation

### 6.3 Misconfigurations

Examples:

- Incorrect firewall rules
- Overprivileged users or groups
- Unnecessary running services

**Mitigation:**

- Configuration management tools
- Regular audits and hardening reviews

### 6.4 Data Exfiltration

- Unauthorized transfer of sensitive data outside the organization.

**Mitigation:**

- Encryption (data at rest and in transit)
- DLP solutions
- Endpoint protection
- Firewall and proxy log analysis

### 6.5 Malicious Updates

- Fake update packages or supply chain attacks.

**Mitigation:**

- Download updates only from trusted sources
- Verify digital signatures and file hashes
- Use application allow-listing

---

## 7. SQL and XML Injection Attacks

### 7.1 Injection Attacks Overview

- Injection attacks involve inserting unexpected commands or malicious input into an application.

---

## 7.2 SQL Injection

### 7.2.1 Basic SQL Operations

- **SELECT** – Retrieve data
- **INSERT** – Add data
- **UPDATE** – Modify data
- **DELETE** – Remove data

### 7.2.2 How SQL Injection Works

- Attackers inject malicious SQL code through:
  - Input fields
  - URL parameters
  - Cookies
  - HTTP headers

Example:

```sql
' OR 1=1 --
```

Possible results:

- Authentication bypass
- Data disclosure
- Data manipulation

### 7.2.3 SQL Injection Mitigations

- Input validation
- Parameterized queries / prepared statements
- Secure stored procedures
- Output encoding
- Web Application Firewall (WAF)

---

## 7.3 XML Injection / XXE

### 7.3.1 XML Basics

- XML is a data exchange format using structured tags.

### 7.3.2 XML-Based Attacks

#### XML Bomb (Billion Laughs)

- Consumes excessive CPU and memory resources, causing DoS.

#### XXE (XML External Entity)

- Attempts to access internal files or trigger SSRF attacks.

### 7.3.3 XML Security Best Practices

- Disable external entities
- Apply strict input validation
- Use secure parser configurations

---

## 8. XSS and CSRF

## 8.1 XSS (Cross-Site Scripting)

### Purpose

Inject malicious scripts into trusted websites.

Possible consequences:

- Session cookie theft
- Performing actions as the victim
- Website defacement

### Types of XSS

| Type | Description |
|------|-------------|
| **Reflected (Non-Persistent)** | Triggered through a single request |
| **Stored (Persistent)** | Stored in the database and executed repeatedly |
| **DOM-Based** | Executed on the client side through DOM manipulation |

### Mitigations

- Input validation
- Output encoding
- Secure frameworks
- Content Security Policy (CSP)

---

## 8.2 Session Management and Cookies

### Session Hijacking

- Attackers steal session IDs to impersonate users.

### Session Prediction

- Attackers predict weak session tokens.

**Mitigation:**

- Use cryptographically secure random tokens

---

## 8.3 CSRF (Cross-Site Request Forgery)

- Tricks authenticated users into performing unwanted actions.

### Mitigations

- Anti-CSRF tokens
- Reauthentication for critical actions
- SameSite cookies
- Multi-factor authentication

---

## 9. Buffer Overflow

### 9.1 Basic Concept

- Writing more data into a buffer than it can hold, overwriting adjacent memory.

### 9.2 Stack and Return Address

Attackers may overwrite:

- Function parameters
- Local variables
- Return addresses

This can redirect execution to malicious code.

### 9.3 Smashing the Stack & NOP Sled

- **Smashing the Stack:** Overwriting the return address.
- **NOP Sled:** A sequence of NOP instructions leading execution to shellcode.

### 9.4 Buffer Overflow Mitigations

- ASLR (Address Space Layout Randomization)
- Stack canaries
- DEP (Data Execution Prevention)
- Secure coding practices

---

## 10. Race Conditions

### 10.1 Definition

- Occurs when multiple threads or processes access shared resources simultaneously, making outcomes dependent on execution timing.

### 10.2 Important Terms

- **TOC (Time of Check)**
- **TOU (Time of Use)**
- **TOE (Time of Evaluation)**

### 10.3 Example

A bank balance is checked, but before the transaction completes, another process changes the balance.

Possible result:

- Unexpected overdrafts
- Inconsistent system behavior

### 10.4 Dirty COW

- A well-known Linux/Android race condition exploit.
- Exploits Copy-On-Write timing issues to gain root privileges.

### 10.5 Race Condition Mitigations

- Locks
- Mutexes
- Proper concurrency design
- Extensive testing for timing-related vulnerabilities
