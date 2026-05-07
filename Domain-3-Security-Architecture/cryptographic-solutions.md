# Cryptographic Solutions

## Overview

Cryptography is the practice of protecting data by ensuring:

- **Confidentiality**
- **Integrity**
- **Authenticity**

It is one of the core foundations of cybersecurity.

---

## Cryptography and Encryption

| Concept | Description |
|---------|-------------|
| **Cryptography** | The science of encoding and decoding information to protect its meaning |
| **Encryption** | The process of converting plaintext into ciphertext |
| **Purpose** | Protects data at rest, in transit, and in use |

---

## Data States

| Data State | Description |
|------------|-------------|
| **Data at Rest** | Data stored on physical or cloud storage systems |
| **Data in Transit** | Data moving across networks |
| **Data in Use** | Data actively being processed |

---

## Algorithm and Key Concepts

| Concept | Description |
|---------|-------------|
| **Algorithm (Cipher)** | A mathematical process used for encryption or decryption |
| **Key** | A secret value used to encrypt or decrypt data |
| **Key Length** | Longer keys generally provide stronger security |
| **Key Rotation** | Periodically replacing cryptographic keys to improve security |

---

## Symmetric vs Asymmetric Encryption

| Type | Description |
|------|-------------|
| **Symmetric Encryption** | Uses the same key for encryption and decryption. Fast but key distribution is challenging |
| **Asymmetric Encryption** | Uses a public and private key pair. More secure for key exchange but slower |
| **Hybrid Encryption** | Uses asymmetric encryption for key exchange and symmetric encryption for data transfer |

---

## Cipher Types

| Type | Description |
|------|-------------|
| **Stream Cipher** | Encrypts data bit-by-bit or byte-by-byte |
| **Block Cipher** | Encrypts data in fixed-size blocks |

---

## Symmetric Encryption Algorithms

| Algorithm | Type | Description |
|-----------|------|-------------|
| **DES** | Block Cipher | 56-bit key, outdated and insecure |
| **3DES** | Block Cipher | Triple DES, stronger than DES but slower |
| **IDEA** | Block Cipher | 128-bit encryption algorithm |
| **AES** | Block Cipher | Modern encryption standard using 128, 192, or 256-bit keys |
| **Blowfish** | Block Cipher | Fast and flexible algorithm |
| **Twofish** | Block Cipher | Open-source and highly secure |
| **RC4** | Stream Cipher | Deprecated and insecure |
| **RC5 / RC6** | Block Cipher | Improved versions of RC algorithms |

---

## Asymmetric Encryption Algorithms

| Algorithm | Use Case | Description |
|-----------|----------|-------------|
| **Diffie-Hellman (DH)** | Key Exchange | Securely exchanges keys between parties |
| **RSA** | Encryption and Digital Signatures | Based on prime number factorization |
| **ECC** | Encryption and Digital Signatures | Provides strong security with smaller key sizes |

### ECC Variants

- **ECDH** → Elliptic Curve Diffie-Hellman (Key Exchange)
- **ECDHE** → Ephemeral Key Exchange
- **ECDSA** → Digital Signatures

---

## Digital Signatures

Digital signatures provide:

- **Integrity**
- **Authentication**
- **Non-Repudiation**

### How Digital Signatures Work

1. A hash is created from the original message
2. The hash is encrypted using the sender's private key
3. The receiver verifies it using the sender's public key

---

## Hashing

| Algorithm | Hash Length | Description |
|-----------|-------------|-------------|
| **MD5** | 128-bit | Deprecated due to collision vulnerabilities |
| **SHA-1** | 160-bit | Deprecated |
| **SHA-2** | 224–512-bit | Modern standard |
| **SHA-3** | Variable | Latest SHA standard |
| **RIPEMD** | 128–320-bit | Alternative hashing algorithm |
| **HMAC** | Variable | Hashing combined with a secret key |

---

## Public Key Infrastructure (PKI)

PKI is a trust framework used for certificate management and key distribution.

| Component | Description |
|-----------|-------------|
| **CA (Certificate Authority)** | Issues and signs digital certificates |
| **RA (Registration Authority)** | Verifies identity before certificate issuance |
| **CSR (Certificate Signing Request)** | Request sent for certificate creation |
| **CRL (Certificate Revocation List)** | List of revoked certificates |
| **OCSP** | Online certificate status validation |

---

## Digital Certificates

| Concept | Description |
|---------|-------------|
| **Root of Trust** | The highest trusted authority in certificate validation |
| **Public Key Pinning** | Prevents certificate spoofing |
| **Key Escrow** | Secure storage of private key backups |
| **Recovery Agents** | Recover encrypted data when keys are lost |

---

## Blockchain

Blockchain is a decentralized and immutable digital ledger.

### Key Characteristics

- Decentralization
- Transparency
- Integrity
- Immutability

### Common Use Cases

| Use Case | Description |
|----------|-------------|
| **Smart Contracts** | Self-executing digital contracts |
| **Commercial Applications** | Enterprise blockchain implementations |
| **Supply Chain Management** | Tracking product origin and movement |

---

## Encryption Tools

| Tool | Description |
|------|-------------|
| **TPM (Trusted Platform Module)** | Hardware-based secure key storage |
| **HSM (Hardware Security Module)** | Dedicated hardware for key protection |
| **KMS (Key Management System)** | Manages the cryptographic key lifecycle |
| **Secure Enclaves** | Isolated processor security environments |

---

## Obfuscation Techniques

| Technique | Description |
|-----------|-------------|
| **Steganography** | Hides data inside another file |
| **Tokenization** | Replaces sensitive data with tokens |
| **Data Masking** | Hides real data for testing or analysis |

---

## Cryptographic Attacks

| Attack | Description |
|--------|-------------|
| **Downgrade Attack** | Forces systems to use weaker protocols |
| **Collision Attack** | Finds two inputs with the same hash |
| **Birthday Attack** | Exploits hash collision probability |

---

## Quantum Computing Threats

Quantum computing may break many traditional encryption algorithms.

### Key Concepts

| Concept | Description |
|---------|-------------|
| **Quantum Computing** | Advanced computing using qubits |
| **Qubit** | Can represent both 0 and 1 simultaneously |
| **Quantum Communication** | Secure communication using quantum states |

### Security Impact

Quantum computing threatens algorithms such as:

- RSA
- ECC

---

## Post-Quantum Cryptography (PQC)

Post-quantum algorithms are designed to resist quantum attacks.

| Category | Examples |
|----------|----------|
| **Encryption** | CRYSTALS-Kyber |
| **Digital Signatures** | CRYSTALS-Dilithium, Falcon, SPHINCS+ |

---

## Important Exam Notes

### Symmetric Encryption

- Uses the same key for encryption and decryption
- Fast but key distribution is difficult

Examples:

- AES
- Blowfish
- Twofish

---

### Asymmetric Encryption

- Uses public and private key pairs
- Solves key distribution challenges

Examples:

- RSA
- ECC

---

### Hashing

Used to verify data integrity.

Examples:

- SHA-2
- SHA-3

Avoid:

- MD5
- SHA-1

---

### Full Disk Encryption (FDE)

Encrypts an entire storage device.

Often used with:

- TPM

---

### Key Protection

- **KMS** → Manages keys
- **HSM** → Protects keys physically

---

## Summary

- Cryptography protects sensitive information
- Symmetric encryption is fast
- Asymmetric encryption is secure for key exchange
- Hashing protects integrity
- PKI establishes trust
- Blockchain provides decentralized trust
- Quantum computing introduces new cryptographic challenges

---
