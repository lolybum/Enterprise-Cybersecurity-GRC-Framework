# STD-014 Enterprise Encryption and Key Management Standard

**Document ID:** STD-014

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-024 Enterprise Security Architecture Policy
- GOV-027 Enterprise Data Protection Policy
- GOV-031 Enterprise Identity and Access Management Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Encryption and Key Management Standard is to establish mandatory technical and operational requirements for the use of cryptography to protect organizational information throughout its lifecycle.

This standard defines enterprise requirements for encryption, cryptographic key management, certificate management, and secure implementation of cryptographic controls to ensure the confidentiality, integrity, authenticity, and availability of enterprise information.

---

# 2. Scope

This standard applies to:

- Servers.
- Workstations.
- Mobile devices.
- Databases.
- Enterprise applications.
- Cloud infrastructure.
- Storage systems.
- Backup systems.
- Virtual machines.
- Containers.
- Identity and Access Management (IAM) systems.
- Public Key Infrastructure (PKI).
- Hardware Security Modules (HSMs).
- APIs.
- SaaS platforms where encryption responsibilities apply.

This standard applies to all organizational data classified as Confidential, Restricted, or otherwise requiring cryptographic protection.

---

# 3. Objectives

The objectives of this standard are to:

- Protect sensitive organizational information.
- Standardize enterprise encryption practices.
- Secure cryptographic key management.
- Support Zero Trust Architecture.
- Strengthen regulatory compliance.
- Protect data confidentiality.
- Preserve data integrity.
- Enable secure authentication.
- Reduce cryptographic risk.
- Improve enterprise cyber resilience.

---

# 4. Standard Statement

The organization shall implement approved cryptographic controls to protect sensitive information at rest, in transit, and, where appropriate, in use.

Encryption technologies, cryptographic algorithms, certificates, and key management processes shall comply with recognized industry standards, applicable regulations, and enterprise security requirements.

Cryptographic keys shall be generated, distributed, stored, rotated, archived, revoked, and destroyed using approved enterprise key management processes.

---

# 5. Encryption Governance

The organization shall establish governance processes to ensure cryptographic controls are consistently implemented, managed, and maintained.

Encryption governance requirements include:

- Approved enterprise cryptographic standards.
- Defined cryptographic ownership.
- Approved encryption technologies.
- Risk-based encryption requirements.
- Cryptographic lifecycle management.
- Periodic cryptographic reviews.
- Compliance with applicable regulations.
- Executive oversight of enterprise cryptographic controls.

Cryptographic controls shall be reviewed at least annually or following significant technology, regulatory, or business changes.

---

# 6. Data-at-Rest Encryption

Sensitive organizational information stored on enterprise systems shall be protected using approved encryption technologies.

Data-at-rest encryption requirements include:

- Full disk encryption for enterprise laptops.
- Encryption of confidential databases.
- Encryption of enterprise backup media.
- Encryption of cloud storage services.
- Encryption of virtual machine storage.
- Encryption of removable storage devices containing organizational information.
- Encryption of file servers containing confidential data.
- Monitoring of encryption status.

Encryption keys shall be managed separately from encrypted data.

---

# 7. Data-in-Transit Encryption

Organizational information transmitted across internal and external networks shall be protected using approved cryptographic protocols.

Requirements include:

- TLS 1.2 or higher as the minimum standard.
- TLS 1.3 where supported.
- HTTPS for web applications.
- Secure Shell (SSH) for administrative access.
- Secure VPN encryption.
- Secure email encryption where required.
- Encryption of API communications.
- Certificate validation.
- Prohibition of deprecated protocols such as SSL, TLS 1.0, and TLS 1.1.

All sensitive network communications shall use encrypted channels.

---

# 8. Approved Cryptographic Algorithms

Only enterprise-approved cryptographic algorithms shall be used to protect organizational information.

Approved algorithms include:

- AES-256 for symmetric encryption.
- RSA-3072 or higher for asymmetric encryption.
- Elliptic Curve Cryptography (ECC) using approved curves.
- SHA-256 or stronger hashing algorithms.
- SHA-384 or SHA-512 where higher assurance is required.
- HMAC-SHA-256 or stronger for message authentication.
- TLS-approved cipher suites.

The use of deprecated or insecure algorithms is prohibited, including:

- DES
- 3DES (except where temporary compatibility is approved)
- RC4
- MD5
- SHA-1 for digital signatures
- Anonymous cipher suites

Exceptions require documented approval through the Enterprise Exception Management process.

---

# 9. Cryptographic Key Generation

Cryptographic keys shall be generated using enterprise-approved methods that provide sufficient entropy and security.

Key generation requirements include:

- Use approved cryptographic random number generators.
- Generate keys using enterprise-approved cryptographic libraries.
- Protect key generation processes from unauthorized access.
- Generate keys with approved key lengths.
- Document key ownership.
- Record key creation dates.
- Assign key expiration periods.
- Restrict key generation to authorized personnel and systems.

Cryptographic keys shall never be generated using predictable or weak methods.

---

# 10. Cryptographic Key Storage

Cryptographic keys shall be securely stored to prevent unauthorized disclosure or compromise.

Key storage requirements include:

- Store keys within approved enterprise key management systems.
- Use Hardware Security Modules (HSMs) where required.
- Encrypt stored cryptographic keys.
- Restrict access using Role-Based Access Control (RBAC).
- Protect key backups.
- Log all administrative access to key repositories.
- Periodically review key access permissions.
- Monitor key storage systems continuously.

Private cryptographic keys shall never be stored in plaintext.