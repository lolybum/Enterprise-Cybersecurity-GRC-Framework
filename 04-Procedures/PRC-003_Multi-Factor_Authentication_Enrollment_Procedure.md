# PRC-003 Multi-Factor Authentication (MFA) Enrollment Procedure

**Procedure ID:** PRC-003

**Version:** 1.0

**Owner:** Identity and Access Management (IAM) Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-031 Enterprise Identity and Access Management Policy
- STD-001 Enterprise Password Standard
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for enrolling users in the organization's Multi-Factor Authentication (MFA) solution to strengthen identity verification and protect enterprise systems from unauthorized access.

This procedure ensures that MFA enrollment is completed consistently, securely, and in compliance with enterprise security requirements.

---

# 2. Scope

This procedure applies to:

- Employees.
- Contractors.
- Consultants.
- Temporary workers.
- Third-party users.
- Service accounts where technically supported.
- Identity and Access Management (IAM) administrators.
- Information Security personnel.

This procedure applies to all enterprise-managed systems requiring Multi-Factor Authentication.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Verify user identity before MFA enrollment.
- Ensure all eligible users are enrolled in MFA.
- Support secure onboarding of authentication devices.
- Protect enterprise accounts from unauthorized access.
- Support regulatory and audit requirements.
- Maintain complete enrollment records.
- Reduce identity-based cyber risks.
- Standardize MFA enrollment across the enterprise.

---

# 4. Prerequisites

Prior to MFA enrollment, the following requirements shall be met:

- The user account has been successfully provisioned.
- The user's identity has been verified.
- The user has completed required onboarding activities.
- The user possesses an approved MFA device or authentication method.
- The account is active and in good standing.
- A valid IT Service Management (ITSM) request exists where required.
- The user has acknowledged the organization's Acceptable Use Policy.

---

# 5. Roles and Responsibilities

## User

The User shall:

- Complete identity verification.
- Register an approved MFA authentication method.
- Protect registered authentication devices.
- Promptly report lost, stolen, or replaced devices.
- Complete MFA enrollment before accessing protected enterprise resources.

## Hiring Manager

The Hiring Manager shall:

- Ensure new personnel complete MFA enrollment during onboarding.
- Verify business need for access.
- Support users experiencing enrollment issues.

## Service Desk

The Service Desk shall:

- Assist users with MFA enrollment.
- Verify user identity before providing assistance.
- Document all MFA enrollment requests.
- Escalate unresolved issues to the IAM Team.

## Identity and Access Management (IAM) Team

The IAM Team shall:

- Administer the enterprise MFA solution.
- Approve supported authentication methods.
- Verify successful MFA enrollment.
- Maintain MFA enrollment records.
- Investigate enrollment failures.
- Support MFA device replacement requests.

## Information Security Team

The Information Security Team shall:

- Monitor MFA enrollment compliance.
- Review MFA security events.
- Investigate suspected MFA compromise.
- Recommend improvements to MFA controls.

---

# 6. Approved MFA Authentication Methods

Only enterprise-approved authentication methods shall be used.

Approved methods include:

- Authenticator application (preferred).
- Hardware security token (FIDO2/WebAuthn).
- Smart card or PIV card.
- Push notification through an approved authenticator application.
- Time-Based One-Time Password (TOTP).
- Certificate-based authentication where approved.

The following methods shall only be used if specifically approved by the Information Security Team:

- SMS verification.
- Voice call verification.

Unapproved authentication methods shall not be used.

---

# 7. User Identity Verification

Prior to MFA enrollment, the user's identity shall be verified using approved enterprise processes.

Identity verification may include:

- Government-issued identification (in person).
- Existing enterprise credentials.
- Human Resources verification.
- Manager confirmation where appropriate.
- Approved identity proofing processes.
- Existing MFA authentication for device replacement requests.

Enrollment shall not proceed until identity verification has been successfully completed.

---

# 8. MFA Enrollment Workflow

### Step 1 – Verify User Eligibility

- Confirm the account is active.
- Confirm the user requires MFA.
- Verify identity.
- Confirm completion of onboarding activities.

---

### Step 2 – Register Authentication Method

- Launch the approved MFA enrollment portal.
- Select an approved authentication method.
- Register the authentication device.
- Generate required enrollment credentials.
- Associate the device with the user's enterprise account.

---

### Step 3 – Configure Security Settings

- Apply enterprise MFA policy.
- Configure authentication prompts.
- Register backup authentication methods where permitted.
- Verify policy synchronization.

---

### Step 4 – Validate Enrollment

- Perform a successful MFA authentication.
- Verify access to enterprise applications.
- Confirm successful enrollment within the MFA management console.
- Document enrollment completion.

---

# 9. Device Registration

Approved authentication devices shall:

- Be uniquely associated with a single user.
- Be registered within the enterprise MFA platform.
- Meet enterprise security requirements.
- Be protected against unauthorized access.
- Be removed promptly when replaced or retired.

Lost or stolen devices shall be reported immediately and removed from the user's account.

---

# 10. Initial Authentication Validation

Following enrollment, the IAM Team or user shall verify:

- Successful MFA authentication.
- Access to authorized applications.
- Proper operation of the registered authentication method.
- Enforcement of MFA policies.
- Successful logging of authentication events.

Enrollment shall not be considered complete until successful authentication has been verified.

---

# 11. Backup Authentication Methods

To ensure business continuity while maintaining strong security controls, users may register approved backup authentication methods.

Requirements include:

- Backup authentication methods shall be approved by the Information Security Team.
- A minimum of one backup authentication method should be registered where technically supported.
- Backup methods shall meet the same security requirements as primary authentication methods.
- Users shall periodically verify that backup authentication methods remain functional.
- Backup authentication methods shall be removed immediately when no longer required.

Examples of approved backup methods include:

- Secondary authenticator application.
- Secondary hardware security key.
- Recovery codes where supported.
- Certificate-based authentication where approved.

Backup authentication methods shall never reduce the overall security posture of the enterprise.

---

# 12. Lost or Stolen Device Procedure

Users shall immediately report any lost, stolen, or compromised MFA device.

The following steps shall be followed:

### Step 1 – Report the Incident

- Notify the Service Desk immediately.
- Report suspected compromise to the Information Security Team.
- Create an IT Service Management (ITSM) ticket.

### Step 2 – Verify Identity

- Complete identity verification.
- Confirm employment status.
- Validate ownership of the affected account.

### Step 3 – Disable the Device

- Remove the lost or stolen device from the MFA platform.
- Invalidate active authentication sessions where appropriate.
- Review recent authentication activity.

### Step 4 – Register a Replacement Device

- Register a new approved authentication device.
- Perform MFA enrollment validation.
- Confirm successful authentication.

All actions shall be documented within the ITSM platform.

---

# 13. MFA Device Replacement

Replacement of MFA devices shall follow an approved verification process.

Requirements include:

- Identity verification prior to replacement.
- Approval by the IAM Team where required.
- Removal of the previous authentication device.
- Registration of the replacement device.
- Validation of successful authentication.
- Documentation of replacement activities.
- Review of recent authentication logs.
- Notification to the user upon completion.

Replacement requests involving privileged accounts shall receive additional security review.

---

# 14. Audit Logging Requirements

All MFA enrollment and management activities shall generate audit records.

Audit logs shall include:

- User identifier.
- Enrollment date and time.
- Authentication method enrolled.
- Administrator performing the action where applicable.
- Device registration events.
- Device replacement events.
- Lost or stolen device reports.
- Successful and failed enrollment attempts.
- Exception approvals.
- Escalation records.

Audit logs shall be protected against unauthorized modification and retained in accordance with the Enterprise Security Logging and Monitoring Standard.

---

# 15. Exception Handling

Exceptions to this procedure shall follow the Enterprise Exception Management process.

Exception requirements include:

- Documented business justification.
- Risk assessment.
- Identification of compensating security controls.
- Approval by the IAM Manager.
- Information Security review where elevated risk exists.
- Defined expiration date.
- Periodic review of approved exceptions.
- Documentation within the Enterprise Exception Register.

Temporary exceptions shall be removed immediately upon expiration.

---

# 16. Escalation Process

Issues identified during MFA enrollment shall be escalated according to organizational procedures.

### Level 1 – Service Desk

Examples:

- Standard enrollment assistance.
- Authentication application installation.
- User guidance.

---

### Level 2 – IAM Team

Examples:

- Enrollment failures.
- Device registration issues.
- Synchronization problems.
- High-risk user requests.

---

### Level 3 – Information Security Team

Examples:

- Suspected MFA compromise.
- Unauthorized enrollment attempts.
- Privileged account enrollment issues.
- Security policy violations.

---

### Level 4 – Chief Information Security Officer (CISO)

Examples:

- Enterprise-wide MFA failures.
- Executive authentication exceptions.
- Regulatory or audit-related concerns.
- Significant cybersecurity incidents involving authentication.

All escalations shall be documented within the approved IT Service Management (ITSM) platform.

---

# 17. Compliance

Compliance with this procedure shall be verified through:

- Internal Identity and Access Management (IAM) audits.
- Multi-Factor Authentication (MFA) enrollment reviews.
- Authentication control assessments.
- Access control compliance reviews.
- Regulatory compliance assessments.
- Executive management reviews.
- Independent assurance activities.
- Periodic audit testing.
- Information Security monitoring.
- Continuous compliance reporting.

Failure to comply with this procedure may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Temporary suspension of enrollment privileges.
- Increased management oversight.
- Formal risk acceptance where appropriate.
- Disciplinary action in accordance with organizational policies.
- Contractual action for third parties where applicable.

---

# 18. Exceptions

Exceptions to this procedure shall:

- Be formally documented.
- Include a valid business justification.
- Include a documented risk assessment.
- Identify compensating security controls.
- Be approved by the IAM Manager.
- Be reviewed by the Information Security Team where elevated risk exists.
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 19. References

This procedure aligns with:

- NIST SP 800-53 Rev. 5 – Identification and Authentication (IA) Control Family
- NIST SP 800-63B – Digital Identity Guidelines: Authentication and Lifecycle Management
- NIST Cybersecurity Framework (CSF) 2.0
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- CIS Controls v8
- Microsoft Entra ID Security Best Practices
- FIDO Alliance Authentication Standards

---

# 20. Related Documents

- GOV-031 Enterprise Identity and Access Management Policy
- STD-001 Enterprise Password Standard
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management Standard
- PRC-001 User Account Provisioning Procedure
- PRC-002 Password Reset Procedure
- PRC-004 Privileged Access Request Procedure

---

# 21. Procedure Review

This procedure shall be reviewed:

- Annually.
- Following significant changes to authentication technologies.
- Following MFA-related security incidents.
- Following audit findings.
- Following regulatory or contractual changes.
- Following significant organizational restructuring.

All revisions shall be documented using the organization's document management process.

---

# 22. Approval

| Role | Approval |
|------|----------|
| Chief Information Security Officer | Approved |
| IAM Manager | Approved |
| Information Security Governance Committee | Approved |

---

# 23. Document Control

| Item | Value |
|------|-------|
| Procedure ID | PRC-003 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Procedure Owner | IAM Manager |
| Status | Approved |

---

**End of Procedure**