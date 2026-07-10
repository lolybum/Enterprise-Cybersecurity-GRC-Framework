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

---

# 11. Cryptographic Key Lifecycle Management

The organization shall manage cryptographic keys throughout their entire lifecycle using documented enterprise key management procedures.

Key lifecycle management requirements include:

- Secure key generation.
- Key registration and inventory management.
- Secure key distribution.
- Controlled key activation.
- Secure operational use.
- Periodic key rotation.
- Key archival where required.
- Key revocation.
- Secure key destruction.
- Documentation of all lifecycle activities.

All cryptographic key lifecycle events shall be logged and subject to periodic review.

---

# 12. Public Key Infrastructure (PKI)

The organization shall implement an enterprise Public Key Infrastructure (PKI) to support digital certificates, authentication, encryption, and digital signatures.

PKI requirements include:

- Approved Certificate Authorities (CAs).
- Secure certificate issuance.
- Certificate lifecycle management.
- Certificate revocation capabilities.
- Certificate renewal procedures.
- Secure storage of private keys.
- Certificate policy documentation.
- Periodic PKI security assessments.
- Protection of Certification Authority infrastructure.
- High availability for critical PKI services.

PKI services shall support enterprise authentication and secure communications.

---

# 13. Certificate Management

Digital certificates shall be managed throughout their lifecycle.

Certificate management requirements include:

- Approved certificate request procedures.
- Identity validation before certificate issuance.
- Automated certificate renewal where supported.
- Monitoring of certificate expiration dates.
- Revocation of compromised certificates.
- Secure certificate storage.
- Inventory of enterprise certificates.
- Removal of expired certificates.
- Documentation of certificate ownership.
- Periodic certificate compliance reviews.

Expired or compromised certificates shall be replaced immediately.

---

# 14. Hardware Security Modules (HSMs)

Hardware Security Modules (HSMs) shall be used where required to protect highly sensitive cryptographic keys.

HSM requirements include:

- Secure cryptographic key generation.
- Secure key storage.
- Hardware-enforced key protection.
- FIPS 140-3 validated HSMs where regulatory or contractual requirements apply.
- Role-based administrative access.
- Multi-factor authentication for HSM administration.
- Audit logging of administrative actions.
- Backup of HSM configurations.
- Secure firmware updates.
- Periodic security assessments.

Access to HSMs shall be limited to authorized personnel.

---

# 15. Key Rotation, Revocation, Backup, and Recovery

Cryptographic keys shall be periodically rotated and securely recoverable when required.

Requirements include:

### Key Rotation

- Rotate keys according to enterprise-defined schedules.
- Rotate keys immediately following suspected compromise.
- Document key rotation activities.
- Validate successful key replacement.

### Key Revocation

- Revoke compromised keys immediately.
- Revoke keys no longer required.
- Publish certificate revocation information where applicable.
- Notify affected system owners.

### Key Backup

- Backup critical cryptographic keys.
- Encrypt key backups.
- Restrict access to key backup media.
- Store backup copies separately from production environments.

### Key Recovery

- Maintain documented recovery procedures.
- Test recovery procedures periodically.
- Require dual authorization for sensitive key recovery activities.
- Log all recovery operations.

---

# 16. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve enterprise cryptographic requirements.
- Review enterprise cryptographic risks.
- Ensure compliance with applicable regulations and security frameworks.

## Information Security Team

The Information Security Team shall:

- Develop cryptographic standards.
- Maintain enterprise encryption requirements.
- Monitor cryptographic compliance.
- Review certificate management activities.
- Validate key management controls.
- Recommend improvements to enterprise cryptographic capabilities.

## Information Technology Team

The Information Technology Team shall:

- Deploy approved encryption technologies.
- Maintain enterprise key management systems.
- Support PKI infrastructure.
- Maintain Hardware Security Modules (HSMs).
- Implement certificate lifecycle management.
- Monitor encryption technologies.

## System Owners

System Owners shall:

- Identify systems requiring encryption.
- Ensure enterprise encryption requirements are implemented.
- Participate in certificate lifecycle activities.
- Support key management reviews.
- Request approved cryptographic exceptions where necessary.

## Users

Users shall:

- Protect cryptographic credentials assigned to them.
- Use approved encrypted communication methods.
- Report suspected key compromise immediately.
- Comply with enterprise encryption requirements.

---

# 17. Compliance

Compliance with this standard shall be verified through:

- Internal security audits.
- External security assessments.
- Cryptographic implementation reviews.
- Encryption compliance assessments.
- Public Key Infrastructure (PKI) reviews.
- Certificate lifecycle management assessments.
- Hardware Security Module (HSM) security reviews.
- Regulatory compliance assessments.
- Executive management reviews.
- Independent assurance activities.

Failure to comply with this standard may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Increased monitoring of cryptographic controls.
- Revocation of unauthorized cryptographic implementations.
- Formal risk acceptance by executive management where appropriate.
- Disciplinary action in accordance with organizational policies.
- Contractual action for third parties where applicable.

---

# 18. Exceptions

Exceptions to this standard shall:

- Be formally documented.
- Include a valid business justification.
- Include a documented risk assessment.
- Identify compensating security controls.
- Be approved by the Chief Information Security Officer (CISO).
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 19. References

This standard aligns with:

- NIST SP 800-53 Rev. 5 – Security and Privacy Controls for Information Systems and Organizations
- NIST SP 800-57 Part 1 Rev. 5 – Recommendation for Key Management
- NIST SP 800-175B Rev. 1 – Guideline for Using Cryptographic Standards
- NIST SP 800-131A Rev. 2 – Transitioning the Use of Cryptographic Algorithms and Key Lengths
- NIST Cybersecurity Framework (CSF) 2.0
- FIPS 140-3 – Security Requirements for Cryptographic Modules
- FIPS 197 – Advanced Encryption Standard (AES)
- RFC 8446 – Transport Layer Security (TLS) 1.3
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022

---

# 20. Related Documents

- GOV-024 Enterprise Security Architecture Policy
- GOV-027 Enterprise Data Protection Policy
- GOV-031 Enterprise Identity and Access Management Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-049 Enterprise Zero Trust Architecture Policy
- STD-001 Enterprise Password Standard
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management (IAM) Standard
- STD-004 Enterprise Privileged Access Management (PAM) Standard
- STD-008 Enterprise Endpoint Protection Standard
- STD-009 Enterprise Network Security Standard
- STD-013 Enterprise Backup and Recovery Standard

---

# 21. Definitions

**Encryption** – The process of converting plaintext into ciphertext using approved cryptographic algorithms to protect information from unauthorized access.

**Cryptographic Key** – A value used by a cryptographic algorithm to encrypt, decrypt, sign, or verify information.

**Key Management** – The processes used to generate, distribute, store, rotate, archive, revoke, recover, and destroy cryptographic keys.

**Public Key Infrastructure (PKI)** – A framework of technologies, policies, and procedures used to issue, manage, distribute, validate, and revoke digital certificates.

**Digital Certificate** – An electronic credential that binds a public cryptographic key to the identity of an individual, system, or service.

**Hardware Security Module (HSM)** – A dedicated hardware device designed to securely generate, store, manage, and protect cryptographic keys.

**Key Rotation** – The scheduled replacement of cryptographic keys to reduce the risk associated with long-term key usage.

---

# 22. Approval

| Role | Approval |
|------|----------|
| Executive Management | Approved |
| Chief Information Security Officer | Approved |
| Information Security Governance Committee | Approved |

---

# 23. Document Control

| Item | Value |
|------|-------|
| Document ID | STD-014 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Standard Owner | Chief Information Security Officer |
| Status | Approved |

---

**End of Document**