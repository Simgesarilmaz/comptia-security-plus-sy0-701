# Domain 3 – Security Architecture

## 3.1 Security Architecture Fundamentals

### What is Security Architecture?

Security Architecture defines the overall design, structure, and behavior of an organization's security environment.

It explains:

- How security controls are designed
- Where security controls are implemented
- How security mechanisms protect organizational assets

---

## On-Premise vs Cloud vs Hybrid

### On-Premise Infrastructure

In an on-premise environment, all infrastructure is managed internally by the organization.

#### Advantages

- Full administrative control
- Customizable security configurations
- Direct control over data and hardware

#### Disadvantages

- High upfront and maintenance costs
- Internal responsibility for patching and hardware upgrades
- Limited scalability

---

### Cloud Computing

Cloud computing delivers computing resources over the internet.

#### Advantages

- Fast deployment
- Elastic scalability
- Lower initial investment

#### Risks

- Multi-tenancy concerns
- Vendor lock-in
- Reduced infrastructure control

---

### Hybrid Solutions

Hybrid environments combine on-premise infrastructure with cloud services.

#### Security Considerations

- Proper storage of sensitive data
- Regulatory and compliance requirements
- Secure integration between environments
- Cost optimization

---

## Important Cloud Security Concepts

- **Availability** → Ensuring systems remain accessible
- **Resilience** → Ability to recover from failures
- **Scalability** → Ability to grow with increased demand
- **Responsiveness** → Ability to respond quickly to workloads
- **Risk Transference** → Some risks are transferred to the cloud service provider
- **Power and Compute Management** → Hardware resources are managed by the cloud provider

---

## Cloud Security Risks

### Shared Physical Server (Multi-Tenancy)

Multiple customers share the same physical infrastructure.

#### Risks

- Isolation failures
- VM escape attacks

#### Security Controls

- Hypervisor hardening
- Isolation testing

---

### Inadequate Virtual Environment Security

Weak virtual machine configurations may lead to unauthorized access.

#### Security Controls

- Secure VM templates
- Patch management
- Network segmentation

---

### User Access Management Issues

Identity and access management failures are among the most common cloud risks.

#### Security Controls

- Multi-Factor Authentication (MFA)
- Principle of Least Privilege
- Role-Based Access Control (RBAC)
- Audit logging

---

### Lack of Up-to-Date Security Measures

Outdated systems create exploitable vulnerabilities.

#### Security Controls

- Patch management
- Security policy updates

---

### Single Point of Failure

Failure of one component may impact the entire service.

#### Security Controls

- Redundancy
- Multi-Availability Zone deployment
- Multi-region architecture

---

### Weak Authentication and Encryption

Weak authentication or encryption may lead to data exposure.

#### Security Controls

- MFA
- Encryption for data at rest and in transit
- Key Management Systems (KMS)
- Hardware Security Modules (HSM)

---

### Data Remnants

Residual data may remain after deletion.

#### Security Controls

- Secure deletion
- Encrypted storage
- Cryptographic key destruction

---

## Virtualization and Containerization

### Virtualization

Virtualization allows multiple virtual machines to run on a single physical server.

#### Hypervisor Types

**Type 1 (Bare Metal)**

Examples:

- VMware ESXi
- Microsoft Hyper-V

**Type 2 (Hosted)**

Examples:

- Oracle VirtualBox
- VMware Workstation

---

### Virtualization Vulnerabilities

Common threats include:

- VM escape
- Privilege escalation
- Live migration interception
- Resource reuse attacks

---

### Virtual Machine Security

Security best practices include:

- Patch management
- Template hardening
- Network segmentation
- Hypervisor security
- Encryption of VM files

---

## Containerization

Containerization packages applications with their dependencies.

Examples include:

- Docker
- Kubernetes

#### Advantages

- Fast startup
- Lightweight deployment
- Portability
- Ideal for microservices

#### Security Risks

- Shared kernel exposure
- Insecure container images
- Kubernetes misconfigurations

#### Security Controls

- Image scanning
- RBAC
- Network policies
- Non-root containers

---

## Microservices Architecture

Microservices break a large application into smaller independent services.

#### Advantages

- Independent scaling
- Independent deployment
- Increased flexibility

#### Risks

- Increased network latency
- Expanded attack surface
- Data consistency challenges
- API security concerns

---

## Network Infrastructure and Separation

### Physical Separation (Air Gap)

Systems are completely isolated physically.

---

### Logical Separation

Systems are separated logically using:

- VLANs
- Access Control Lists (ACLs)
- Firewalls

---

## Software-Defined Networking (SDN)

In Software-Defined Networking, the control plane is centralized.

A controller manages network traffic dynamically.

---

## Infrastructure as Code (IaC)

Infrastructure is managed using code.

Common formats include:

- YAML
- JSON
- HCL

#### Benefits

- Standardization
- Speed
- Consistency
- Easier auditing

---

## Centralized vs Decentralized Architecture

### Centralized Architecture

Advantages:

- Easier control
- Simplified management

Risks:

- Single point of failure

---

### Decentralized Architecture

Advantages:

- Greater resilience
- Distributed operations

Risks:

- Increased complexity

---

## Internet of Things (IoT)

IoT refers to interconnected devices that include sensors, software, and network connectivity.

#### Security Risks

- Weak default configurations
- Open ports
- Unencrypted traffic

---

## ICS and SCADA

Industrial Control Systems (ICS) and Supervisory Control and Data Acquisition (SCADA) systems are used in industrial environments.

#### Security Risks

- Unauthorized access
- Malware infections
- Legacy systems without patches

---

## Embedded Systems

Embedded systems are devices designed for specific operational tasks.

#### Security Risks

- Hardware failures
- Software vulnerabilities
- Difficult patching processes

#### Security Controls

- Firmware signing
- Network segmentation
- Secure Over-the-Air (OTA) updates

---
