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