# STD-001 Enterprise Password Standard

**Document ID:** STD-001

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-031 Enterprise Identity and Access Management (IAM) Policy
- GOV-032 Enterprise Password Management Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Password Standard is to establish mandatory password requirements that protect organizational accounts, systems, applications, and information assets from unauthorized access.

This standard defines the minimum password controls required across the enterprise to support secure authentication, reduce credential-related risks, and comply with applicable cybersecurity frameworks, regulatory requirements, and industry best practices.

---

# 2. Scope

This standard applies to:

- All employees.
- Contractors.
- Consultants.
- Temporary workers.
- Third-party users with authorized access.
- Service accounts.
- Privileged accounts.
- Administrative accounts.
- Cloud accounts.
- On-premises systems.
- Mobile devices.
- Enterprise applications.
- Identity providers.

This standard applies to all enterprise authentication systems that utilize passwords or passphrases.

---

# 3. Objectives

The objectives of this standard are to:

- Establish minimum password security requirements.
- Protect enterprise user accounts.
- Reduce credential compromise.
- Support Zero Trust security principles.
- Strengthen identity verification.
- Promote strong authentication practices.
- Support regulatory compliance.
- Reduce unauthorized access.
- Improve enterprise security posture.
- Standardize password requirements across the organization.

---

# 4. Standard Statement

The organization shall enforce standardized password requirements for all enterprise systems, applications, cloud services, and authentication platforms.

Passwords shall be created, stored, transmitted, and managed using secure methods that minimize the risk of compromise.

Where supported, password-based authentication shall be strengthened through Multi-Factor Authentication (MFA) and integrated with the organization's Identity and Access Management (IAM) program.

Enterprise systems shall enforce technical controls to ensure compliance with this standard.

---

# 5. Password Length Requirements

The following minimum password length requirements shall apply:

- User accounts shall use passwords or passphrases with a minimum length of 14 characters.
- Privileged accounts shall use passwords with a minimum length of 16 characters.
- Service accounts shall use passwords with a minimum length of 20 characters.
- Default vendor passwords shall be changed before systems are placed into production.
- Passwords shall not exceed system-supported limits but should support long passphrases where technically feasible.

Longer passphrases are encouraged to improve resistance against brute-force and password guessing attacks.

---

# 6. Password Complexity Requirements

Passwords shall meet the following complexity requirements where technically supported:

- Contain uppercase letters.
- Contain lowercase letters.
- Contain numeric characters.
- Contain special characters.
- Avoid dictionary words used alone.
- Avoid predictable keyboard patterns.
- Avoid common passwords.
- Avoid user names.
- Avoid company names.
- Avoid personal information.

Where modern authentication platforms support passphrases, longer passphrases shall be preferred over overly complex short passwords in accordance with NIST guidance.

---

# 7. Password Storage Requirements

Passwords shall never be stored in plaintext.

Approved password storage methods include:

- One-way salted hashing.
- Approved cryptographic algorithms.
- Secure credential vaults.
- Enterprise password managers.
- Hardware Security Modules (HSMs) where applicable.

The following storage practices are prohibited:

- Plaintext files.
- Shared spreadsheets.
- Email messages.
- Sticky notes.
- Browsers without enterprise management.
- Source code repositories.

---

# 8. Password History

Enterprise authentication systems shall maintain password history controls.

Requirements include:

- Prevent reuse of the previous 24 passwords where technically feasible.
- Prevent immediate password reuse.
- Validate password uniqueness during password changes.
- Enforce password history for privileged accounts.
- Monitor repeated password reuse attempts.

---

# 9. Password Expiration

Routine password expiration shall not be required for standard user accounts unless:

- A password compromise is suspected.
- A security incident occurs.
- Regulatory requirements require password changes.
- Administrative action requires credential rotation.

Privileged accounts and service accounts shall follow organization-approved credential rotation schedules based on risk.

---

# 10. Password Reset Requirements

Password reset processes shall:

- Verify user identity before resetting credentials.
- Require Multi-Factor Authentication (MFA) where supported.
- Generate temporary passwords securely.
- Require password changes upon first login.
- Log all password reset activities.
- Prevent unauthorized password resets.
- Follow documented service desk procedures.

All password reset activities shall be auditable.