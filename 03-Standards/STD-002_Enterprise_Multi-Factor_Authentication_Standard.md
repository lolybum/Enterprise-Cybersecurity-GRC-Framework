# STD-002 Enterprise Multi-Factor Authentication Standard

**Document ID:** STD-002

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-031 Enterprise Identity and Access Management (IAM) Policy
- GOV-032 Enterprise Password Management Policy
- GOV-044 Enterprise Remote Access Security Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Multi-Factor Authentication (MFA) Standard is to establish mandatory requirements for implementing Multi-Factor Authentication across enterprise systems, applications, cloud services, and remote access environments.

This standard defines the minimum authentication requirements necessary to reduce the risk of unauthorized access resulting from compromised credentials and to strengthen identity verification in support of the organization's Zero Trust Architecture.

---

# 2. Scope

This standard applies to:

- All employees.
- Contractors.
- Consultants.
- Temporary workers.
- Third-party users with authorized access.
- Administrative accounts.
- Privileged accounts.
- Remote users.
- Cloud applications.
- Enterprise applications.
- VPN connections.
- Identity providers.
- Systems supporting Multi-Factor Authentication.

This standard applies to all enterprise authentication mechanisms where MFA is technically supported.

---

# 3. Objectives

The objectives of this standard are to:

- Establish mandatory Multi-Factor Authentication requirements.
- Strengthen user identity verification.
- Protect privileged accounts.
- Reduce unauthorized access.
- Support Zero Trust security principles.
- Improve enterprise cyber resilience.
- Protect cloud and remote access environments.
- Support regulatory compliance.
- Standardize authentication controls across the organization.
- Reduce risks associated with credential theft and phishing.

---

# 4. Standard Statement

The organization shall require Multi-Factor Authentication (MFA) for access to enterprise systems, applications, cloud services, remote access solutions, privileged accounts, and other high-risk resources where technically feasible.

MFA shall use at least two independent authentication factors from different categories, such as:

- Something you know (password or PIN).
- Something you have (security token, authenticator application, or smart card).
- Something you are (biometric authentication).

SMS-based authentication should be avoided where stronger authentication methods are available.

Enterprise authentication systems shall enforce MFA in accordance with organizational risk assessments and regulatory requirements.

---

# 5. Multi-Factor Authentication Requirements

The organization shall require Multi-Factor Authentication (MFA) for all systems and services that support MFA capabilities.

MFA shall be mandatory for:

- Administrative accounts.
- Privileged accounts.
- Remote access connections.
- Virtual Private Network (VPN) access.
- Cloud services.
- Software-as-a-Service (SaaS) applications.
- Email systems.
- Identity providers.
- Financial systems.
- Systems processing confidential or regulated information.

Where MFA cannot be implemented due to technical limitations, a documented exception shall be approved by the Chief Information Security Officer (CISO).

---

# 6. Approved Authentication Methods

The organization shall use approved authentication factors from at least two independent categories.

Approved authentication methods include:

### Something You Know

- Password
- Passphrase
- Personal Identification Number (PIN)

### Something You Have

- Authenticator application
- Hardware security token
- Smart card
- FIDO2 security key
- Enterprise-issued cryptographic token

### Something You Are

- Fingerprint
- Facial recognition
- Iris recognition
- Other approved biometric methods

SMS-based authentication shall only be used where stronger authentication methods are not technically feasible.

---

# 7. Enrollment Requirements

Users shall complete the MFA enrollment process before being granted access to enterprise resources requiring MFA.

Enrollment requirements include:

- Identity verification before enrollment.
- Registration of approved authentication devices.
- Validation of recovery methods.
- Acceptance of applicable security policies.
- Confirmation of successful enrollment.
- Secure storage of recovery codes where applicable.

Enrollment records shall be maintained for audit purposes.

---

# 8. MFA for Remote Access

Multi-Factor Authentication shall be required for all remote access to enterprise resources.

This includes:

- Virtual Private Network (VPN) access.
- Remote desktop services.
- Cloud-hosted applications.
- Administrative remote access.
- Third-party remote access.
- Remote support tools.

Remote access sessions shall be authenticated using MFA before access is granted.

---

# 9. MFA for Privileged Accounts

All privileged accounts shall use Multi-Factor Authentication without exception unless a documented risk-based exception has been approved.

Requirements include:

- MFA for all administrative logins.
- MFA for privileged cloud accounts.
- MFA for privileged service management platforms.
- MFA for privileged remote access.
- MFA for infrastructure administration.
- MFA for identity management systems.

Privileged account authentication shall be continuously monitored by the Information Security team.

---

# 10. MFA Exception Requirements

Requests for exceptions to this standard shall:

- Be documented.
- Include business justification.
- Include a documented risk assessment.
- Identify compensating security controls.
- Be approved by the Chief Information Security Officer (CISO).
- Include an expiration date.
- Be reviewed annually.

Approved exceptions shall be recorded in the Enterprise Exception Register.

---

# 11. Administrative Account Requirements

Administrative accounts shall be protected using enhanced authentication controls.

Requirements include:

- Multi-Factor Authentication (MFA) shall be mandatory for all administrative accounts.
- Administrative accounts shall use enterprise-approved MFA methods.
- Shared administrative accounts shall be prohibited unless explicitly approved.
- Administrative authentication events shall be logged.
- Administrative sessions shall automatically timeout after periods of inactivity.
- Administrative access shall follow the principle of least privilege.
- Emergency administrative accounts shall be documented and monitored.
- Administrative authentication shall be continuously monitored for suspicious activity.

---

# 12. Cloud Application Requirements

All enterprise cloud applications shall enforce Multi-Factor Authentication where technically supported.

Cloud authentication requirements include:

- MFA for Software-as-a-Service (SaaS) applications.
- MFA for cloud management consoles.
- MFA for cloud administrators.
- MFA for cloud-based email platforms.
- MFA for enterprise collaboration platforms.
- MFA for cloud storage services.
- Integration with enterprise Identity and Access Management (IAM) systems.
- Continuous monitoring of cloud authentication events.

Cloud applications shall comply with enterprise identity governance requirements.

---

# 13. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve enterprise MFA requirements.
- Review MFA-related risks.
- Ensure alignment with applicable regulations and security frameworks.

## Information Security Team

The Information Security Team shall:

- Maintain the MFA standard.
- Monitor compliance with MFA requirements.
- Review authentication-related security events.
- Recommend improvements to authentication controls.
- Support MFA awareness and training initiatives.

## Information Technology Team

The Information Technology Team shall:

- Implement and maintain enterprise MFA solutions.
- Configure authentication systems.
- Support secure enrollment and recovery processes.
- Maintain authentication infrastructure.
- Monitor operational effectiveness of MFA technologies.

## Managers

Managers shall:

- Ensure personnel comply with MFA requirements.
- Support timely onboarding and offboarding activities.
- Report suspected authentication security issues.

## Users

Users shall:

- Enroll in enterprise MFA as required.
- Protect authentication devices and credentials.
- Immediately report lost or stolen authentication devices.
- Use only approved authentication methods.
- Report suspected account compromise without delay.

---

# 14. Authentication Device Management

Authentication devices shall be securely managed throughout their lifecycle.

Requirements include:

- Registration of enterprise-approved devices.
- Protection of authentication devices from unauthorized use.
- Secure replacement of lost or stolen devices.
- Immediate reporting of compromised authentication devices.
- Periodic review of registered authentication devices.
- Secure disposal of retired authentication devices.
- Revocation of authentication devices upon user separation.

Authentication device inventories shall be maintained by the Information Technology team where applicable.

---

# 15. Compliance

Compliance with this standard shall be verified through:

- Internal security audits.
- External audits.
- Identity and Access Management (IAM) reviews.
- Multi-Factor Authentication (MFA) configuration assessments.
- Privileged Access Management (PAM) reviews.
- Security control testing.
- Vulnerability assessments.
- Continuous monitoring.
- Regulatory compliance reviews.
- Periodic management reviews.

Failure to comply with this standard may result in:

- Corrective action plans.
- Suspension or revocation of system access.
- Mandatory security awareness training.
- Disciplinary action in accordance with organizational policies.
- Contractual action for third parties where applicable.

---

# 16. Exceptions

Exceptions to this standard shall:

- Be formally documented.
- Include a valid business justification.
- Include a documented risk assessment.
- Identify compensating security controls.
- Be approved by the Chief Information Security Officer (CISO).
- Include an expiration date.
- Be reviewed annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 17. References

This standard aligns with:

- NIST SP 800-63B – Digital Identity Guidelines
- NIST SP 800-53 Rev. 5
- NIST Cybersecurity Framework (CSF) 2.0
- NIST SP 800-207 – Zero Trust Architecture
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- CIS Controls v8
- Microsoft Security Baselines
- FIDO Alliance Authentication Standards

---

# 18. Related Documents

- GOV-031 Enterprise Identity and Access Management (IAM) Policy
- GOV-032 Enterprise Password Management Policy
- GOV-033 Enterprise Privileged Access Management (PAM) Policy
- GOV-044 Enterprise Remote Access Security Policy
- GOV-049 Enterprise Zero Trust Architecture Policy
- STD-001 Enterprise Password Standard
- Enterprise Identity and Access Management Standard

---

# 19. Definitions

**Multi-Factor Authentication (MFA)** – An authentication method that requires two or more independent verification factors before granting access to systems or data.

**Authentication Factor** – A category of credentials used to verify identity, such as something you know, something you have, or something you are.

**Authenticator Application** – A software application that generates time-based or event-based one-time passcodes for authentication.

**Privileged Account** – An account with elevated permissions used to administer systems, applications, or security controls.

**Identity Provider (IdP)** – A service that authenticates users and provides identity information to enterprise applications and services.

**FIDO2 Security Key** – A hardware-based authentication device that supports phishing-resistant authentication using public key cryptography.

---

# 20. Approval

| Role | Approval |
|------|----------|
| Executive Management | Approved |
| Chief Information Security Officer | Approved |
| Information Security Governance Committee | Approved |

---

# 21. Document Control

| Item | Value |
|------|-------|
| Document ID | STD-002 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Standard Owner | Chief Information Security Officer |
| Status | Approved |

---

**End of Document**