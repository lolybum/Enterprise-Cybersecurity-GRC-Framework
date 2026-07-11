# PRC-002 Password Reset Procedure

**Procedure ID:** PRC-002

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

The purpose of this procedure is to establish a secure, standardized process for resetting user passwords while protecting enterprise systems from unauthorized access.

This procedure ensures that password reset requests are verified, authorized, documented, and completed in accordance with enterprise security requirements.

---

# 2. Scope

This procedure applies to:

- Employees.
- Contractors.
- Consultants.
- Temporary workers.
- Third-party users.
- Service desk personnel.
- Identity and Access Management (IAM) administrators.
- Information Security personnel.

This procedure applies to all enterprise-managed systems requiring user authentication.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Verify user identity before password reset.
- Prevent unauthorized password changes.
- Support secure self-service password reset.
- Ensure compliance with enterprise password policies.
- Enforce Multi-Factor Authentication (MFA) where required.
- Maintain complete audit records.
- Reduce account compromise risk.
- Support regulatory compliance.

---

# 4. Prerequisites

Prior to resetting a password, the following requirements shall be met:

- A valid password reset request has been received.
- The requestor's identity has been verified.
- The account is active and not disabled.
- The account owner has completed identity verification requirements.
- MFA verification has been completed where applicable.
- The Service Desk ticket or ITSM request has been created.
- Emergency password reset requests have received appropriate approval.

---

# 5. Roles and Responsibilities

## User

The User shall:

- Submit a password reset request through an approved method.
- Complete identity verification requirements.
- Protect temporary passwords from unauthorized disclosure.
- Change the temporary password immediately upon first login.
- Report any suspected unauthorized password reset activity immediately.

## Service Desk

The Service Desk shall:

- Receive password reset requests.
- Verify the requestor's identity.
- Initiate password resets for authorized requests.
- Document all password reset activities.
- Escalate suspicious requests to the IAM Team or Information Security Team.

## Identity and Access Management (IAM) Team

The IAM Team shall:

- Manage password reset processes.
- Support complex password reset requests.
- Enforce enterprise password policies.
- Verify Multi-Factor Authentication (MFA) requirements.
- Review password reset logs.
- Investigate unusual password reset activity.

## Information Security Team

The Information Security Team shall:

- Monitor password reset activities for suspicious behavior.
- Investigate suspected account compromise.
- Support incident response activities.
- Review password reset compliance metrics.

---

# 6. Identity Verification Process

Prior to resetting a password, the requestor's identity shall be verified using approved methods.

Approved identity verification methods include:

- Multi-Factor Authentication (MFA).
- Government-issued identification for in-person requests.
- Verification through Human Resources records where appropriate.
- Employee identification number.
- Verification through approved HR or IAM systems.
- Manager confirmation for exceptional circumstances.

The following methods shall **not** be used as the sole means of identity verification:

- Username only.
- Email address only.
- Caller ID.
- Easily obtainable personal information.

Password resets shall not proceed until identity verification has been successfully completed.

---

# 7. Self-Service Password Reset (SSPR)

Where supported, users shall use the approved Self-Service Password Reset (SSPR) solution.

SSPR requirements include:

- Successful identity verification.
- MFA validation.
- Compliance with password complexity requirements.
- Password history enforcement.
- Minimum password age enforcement where applicable.
- Logging of all reset activities.
- User notification upon successful password reset.

Self-service password reset shall be the preferred method for standard user accounts.

---

# 8. Help Desk Password Reset Workflow

Where self-service password reset is unavailable or unsuccessful, the Help Desk shall perform the password reset.

Workflow:

### Step 1 – Receive Request

- Verify the Service Desk ticket.
- Confirm the requestor's identity.
- Review account status.

### Step 2 – Validate Authorization

- Confirm the account is active.
- Verify that the request complies with enterprise policy.
- Confirm no active security investigation prevents the reset.

### Step 3 – Reset Password

- Generate a temporary password.
- Apply password policy settings.
- Require password change at next login.
- Unlock the account where appropriate.

### Step 4 – Notify User

- Notify the user through an approved communication channel.
- Never transmit passwords through unsecured communication methods.
- Confirm successful user authentication after the reset.

---

# 9. Temporary Password Requirements

Temporary passwords shall:

- Be randomly generated.
- Meet enterprise password complexity requirements.
- Be unique.
- Expire after first successful use.
- Require immediate password change.
- Never be reused.
- Never be stored in plain text.
- Never be shared through unauthorized communication channels.

Temporary passwords shall only be communicated using approved secure methods.

---

# 10. Multi-Factor Authentication (MFA) Verification

Where MFA is required:

- Verify the user's registered MFA device.
- Confirm successful MFA authentication.
- Verify any requested MFA device changes through an approved process.
- Escalate requests involving lost or replaced MFA devices.
- Log all MFA-related password reset activities.

If MFA verification cannot be completed, the password reset request shall be escalated to the IAM Team for additional verification.

---

# 11. Password Policy Validation

All password resets shall comply with the Enterprise Password Standard.

Validation requirements include:

- Minimum password length requirements.
- Password complexity enforcement.
- Password history enforcement.
- Minimum password age where applicable.
- Maximum password age where applicable.
- Prevention of commonly used passwords.
- Prevention of compromised passwords where supported.
- Compliance with enterprise authentication requirements.

Passwords that do not meet enterprise policy shall be rejected automatically.

---

# 12. Account Lockout Handling

Locked accounts shall be managed using approved security procedures.

Account lockout requirements include:

- Verify the user's identity before unlocking an account.
- Determine the reason for the lockout.
- Review recent authentication attempts.
- Check for indicators of unauthorized access.
- Unlock the account only after verification is complete.
- Require a password reset where suspicious activity is identified.
- Escalate suspected account compromise to the Information Security Team.
- Document all account unlock activities.

Repeated account lockouts shall be investigated for potential malicious activity.

---

# 13. Audit Logging Requirements

All password reset activities shall be logged to support security monitoring, investigations, and compliance reviews.

Audit logs shall include:

- Service request or ticket number.
- User identifier.
- Administrator performing the reset.
- Date and time of the reset.
- Identity verification method used.
- MFA verification status.
- Account lockout status.
- Password reset outcome.
- Systems affected.
- Escalation details where applicable.

Audit logs shall be retained and protected in accordance with the Enterprise Security Logging and Monitoring Standard.

---

# 14. Exception Handling

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

# 15. Escalation Process

Password reset issues shall be escalated according to organizational procedures.

### Level 1 – Service Desk

Examples:

- Standard password reset requests.
- Account lockout assistance.
- Self-Service Password Reset (SSPR) support.

---

### Level 2 – IAM Team

Examples:

- Failed identity verification.
- MFA enrollment issues.
- Directory service synchronization problems.
- High-risk user account requests.

---

### Level 3 – Information Security Team

Examples:

- Suspected account compromise.
- Repeated failed authentication attempts.
- Privileged account password resets.
- Security policy violations.

---

### Level 4 – Chief Information Security Officer (CISO)

Examples:

- Executive account password resets requiring exceptions.
- Enterprise-wide authentication failures.
- Regulatory or audit-related concerns.
- Significant cybersecurity incidents affecting authentication services.

All escalations shall be documented within the approved IT Service Management (ITSM) platform.

---

# 16. Documentation and Record Retention

The following records shall be maintained:

- Password reset requests.
- Identity verification records.
- Service Desk tickets.
- IAM administrative actions.
- MFA verification records.
- Audit logs.
- Exception approvals.
- Escalation records.
- Investigation notes where applicable.
- Password reset verification results.

Records shall be retained in accordance with the organization's Records Retention Policy and applicable legal, regulatory, and contractual requirements.