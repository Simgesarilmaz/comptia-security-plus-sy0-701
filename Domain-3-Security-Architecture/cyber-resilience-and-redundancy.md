# Cyber Resilience and Redundancy

## Cyber Resilience

### Definition

Cyber resilience is the ability of systems and organizations to continue operating during cyberattacks, failures, or service disruptions.

### Why It Matters

- **Continuous Operations** → Maintains business operations
- **Swift Recovery** → Enables rapid recovery after incidents
- **Reduced Downtime** → Minimizes service interruptions
- **Minimized Impact** → Reduces operational disruption

---

## Redundancy

### Definition

Redundancy means maintaining duplicate critical components to eliminate single points of failure.

### Examples

- Redundant power supplies
- Redundant network paths
- Redundant servers
- Multi-cloud systems
- Redundant software services

### Objective

Eliminate **Single Points of Failure (SPOF)**.

---

## High Availability (HA)

### Objective

High Availability ensures systems and services remain operational with minimal downtime.

### Common Components

- Load balancing
- Clustering
- Redundant power
- Redundant network connections
- Redundant servers and services
- Multi-cloud architecture

---

## Uptime Standards

| Availability | Downtime |
|--------------|----------|
| **99.999% (Five Nines)** | Approximately 5 minutes per year |
| **99.9999% (Six Nines)** | Approximately 31 seconds per year |

---

## Load Balancing

Load balancing distributes traffic across multiple servers.

### Benefits

- Prevents server overload
- Improves scalability
- Increases availability

---

## Clustering

Clustering allows multiple systems to operate as a single logical system.

### Benefits

- Automatic failover
- Improved uptime
- Higher reliability

---

## Multi-Cloud

Multi-cloud uses services from multiple cloud providers.

Examples:

- AWS
- Microsoft Azure

### Benefits

- Reduces vendor lock-in
- Improves disaster resilience
- Provides flexibility
- Supports cost optimization

---

## Data Redundancy and RAID

### RAID 0 – Striping

Characteristics:

- High performance
- No redundancy

**Exam Tip:** Performance only.

---

### RAID 1 – Mirroring

Characteristics:

- Exact disk duplication
- High redundancy
- Survives one disk failure

---

### RAID 5 – Striping with Parity

Requirements:

- Minimum 3 disks

Characteristics:

- Tolerates 1 disk failure
- Good read performance
- Slower write performance

Common enterprise solution.

---

### RAID 6 – Double Parity

Requirements:

- Minimum 4 disks

Characteristics:

- Tolerates 2 disk failures
- More fault tolerant than RAID 5

---

### RAID 10 (1+0)

Characteristics:

- Combines mirroring and striping
- High performance
- High fault tolerance

Requirements:

- Minimum 4 disks

---

## Capacity Planning

Capacity planning ensures organizations can meet future operational requirements without service disruption.

### Core Areas

#### People

- Staffing requirements
- Skills and training

#### Technology

- Systems
- Applications
- Network resources

#### Infrastructure

- Data centers
- Physical space
- Cooling
- Power systems

#### Processes

- Workflow optimization
- Automation
- Operational efficiency

---

## Power Protection Components

### Line Conditioner

Protects against:

- Voltage sags
- Voltage surges
- Undervoltage

Purpose:

- Stabilizes power quality

---

### UPS (Uninterruptible Power Supply)

Provides battery-backed power during outages.

Typical duration:

- 15 to 60 minutes

Functions:

- Temporary power
- Power conditioning

---

### Generators

Provide long-term backup power during extended outages.

---

### PDC (Power Distribution Center)

Functions:

- Power distribution
- Load balancing
- Integration with UPS and generators

---

## Data Backups

### Backup Locations

- Onsite
- Offsite
- Cloud-based

---

## Backup Components

### Encryption

Protects backup data:

- At rest
- In transit

### Snapshots

Point-in-time copies of systems or data.

### Replication

Real-time duplication of data.

### Journaling

Maintains transaction logs for recovery.

### Recovery Procedures

Defines restoration steps.

---

## Recovery Point Objective (RPO)

RPO defines the maximum acceptable amount of data loss measured in time.

---

## Backup Site Options

| Site Type | Description |
|-----------|-------------|
| **Hot Site** | Fully operational and immediately available |
| **Warm Site** | Partially prepared, operational within days |
| **Cold Site** | Empty facility, requires full setup |
| **Mobile Site** | Portable recovery solution |
| **Virtual Site** | Cloud-based recovery environment |

---

## Geographic Dispersion

Geographic dispersion distributes infrastructure across multiple locations.

### Benefits

- Reduces regional disaster risk
- Improves resilience

---

## Continuity of Operations

### Business Continuity Plan (BCP)

Focuses on maintaining critical business operations during disruptions.

Includes:

- Preventive controls
- Recovery strategies

---

### Disaster Recovery Plan (DRP)

Focuses on restoring technical systems after failures.

Characteristics:

- Technical recovery procedures
- Subset of business continuity planning

---

## Resilience and Recovery Testing

### Tabletop Exercises

Teams discuss response strategies using simulated scenarios.

Characteristics:

- No live systems involved

---

### Failover Testing

Tests switching from primary systems to backup systems.

Characteristics:

- Highly realistic testing

---

### Simulations

Simulated attacks or failures in controlled environments.

---

### Parallel Processing

Primary and secondary systems operate simultaneously.

Benefits:

- Tests resilience
- Validates recovery processes

---

## Important Exam Notes

| Scenario | Best Answer |
|----------|--------------|
| Increase availability | Load Balancer or Clustering |
| Reduce single point of failure | Redundancy |
| Tolerate two disk failures | RAID 6 |
| Immediate disaster recovery site | Hot Site |
| Data loss tolerance | RPO |
| Short-term power protection | UPS |
| Long-term power protection | Generator |

---
