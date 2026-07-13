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