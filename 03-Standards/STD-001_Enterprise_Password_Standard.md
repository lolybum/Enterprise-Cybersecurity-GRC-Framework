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

---

# 11. Service Account Password Requirements

Service account credentials shall be managed using secure enterprise processes.

Requirements include:

- Service accounts shall have unique passwords.
- Passwords shall be a minimum of 20 characters.
- Interactive logon shall be prohibited unless explicitly authorized.
- Passwords shall be stored in approved enterprise credential vaults.
- Password rotation shall occur in accordance with organizational risk requirements.
- Shared service account passwords shall be prohibited where technically feasible.
- Service account ownership shall be documented.
- Unused service accounts shall be disabled or removed promptly.

Service account credentials shall be monitored and reviewed periodically.

---

# 12. Privileged Account Password Requirements

Privileged accounts shall be subject to enhanced password protection controls.

Requirements include:

- Minimum password length of 16 characters.
- Multi-Factor Authentication (MFA) shall be required.
- Privileged credentials shall be managed through an approved Privileged Access Management (PAM) solution where available.
- Administrative passwords shall not be shared.
- Emergency privileged accounts shall be documented and monitored.
- Privileged password usage shall be logged.
- Privileged credentials shall be rotated based on organizational risk.
- Access shall follow the principle of least privilege.

Privileged account activity shall be continuously monitored by the Information Security team.

---

# 13. Enterprise Password Managers

The organization shall approve enterprise password management solutions for storing and managing credentials.

Approved password manager requirements include:

- Strong encryption for stored credentials.
- Multi-Factor Authentication (MFA).
- Secure password generation.
- Role-based administrative controls.
- Secure synchronization where approved.
- Audit logging.
- Secure credential sharing capabilities.
- Backup and recovery support.

The use of unauthorized password management applications is prohibited.

---

# 14. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve password security requirements.
- Review password-related risks.
- Ensure compliance with applicable regulations and frameworks.

## Information Security Team

The Information Security Team shall:

- Maintain password security standards.
- Monitor compliance.
- Review password-related security events.
- Recommend improvements.
- Support password security awareness initiatives.

## Information Technology Team

The Information Technology Team shall:

- Implement technical password controls.
- Configure enterprise authentication systems.
- Maintain password management infrastructure.
- Support secure password reset processes.
- Monitor system compliance.

## Managers

Managers shall:

- Ensure personnel comply with this standard.
- Support timely removal of unnecessary account access.
- Report suspected credential misuse.

## Users

Users shall:

- Create and maintain strong passwords.
- Protect authentication credentials.
- Never share passwords.
- Use approved password managers where required.
- Immediately report suspected credential compromise.

---

# 15. Compliance

Compliance with this standard shall be verified through:

- Internal security audits.
- External audits.
- Identity and Access Management (IAM) reviews.
- Password policy configuration reviews.
- Privileged Access Management (PAM) assessments.
- Security control testing.
- Vulnerability assessments.
- Continuous monitoring.
- Regulatory compliance reviews.
- Periodic management reviews.

Failure to comply with this standard may result in:

- Corrective action plans.
- Mandatory password reset.
- Suspension or revocation of system access.
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

Approved exceptions shall be maintained in the Enterprise Exception Register.

---

# 17. References

This standard aligns with:

- NIST SP 800-63B – Digital Identity Guidelines
- NIST SP 800-53 Rev. 5
- NIST Cybersecurity Framework (CSF) 2.0
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- CIS Controls v8
- Microsoft Security Baselines
- Center for Internet Security (CIS) Benchmarks

---

# 18. Related Documents

- GOV-031 Enterprise Identity and Access Management (IAM) Policy
- GOV-032 Enterprise Password Management Policy
- GOV-033 Enterprise Privileged Access Management (PAM) Policy
- GOV-049 Enterprise Zero Trust Architecture Policy
- Enterprise Multi-Factor Authentication Standard
- Enterprise Privileged Access Standard

---

# 19. Definitions

**Password** – A secret string of characters used to authenticate a user's identity.

**Passphrase** – A longer sequence of words or characters used in place of a traditional password to improve security.

**Multi-Factor Authentication (MFA)** – An authentication method requiring two or more independent verification factors before granting access.

**Privileged Account** – An account with elevated permissions that can administer systems, applications, or security settings.

**Service Account** – A non-interactive account used by applications, services, or automated processes to perform authorized tasks.

**Password Manager** – An approved application used to securely generate, store, and manage passwords and other credentials.

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
| Document ID | STD-001 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Standard Owner | Chief Information Security Officer |
| Status | Approved |

---

**End of Document**