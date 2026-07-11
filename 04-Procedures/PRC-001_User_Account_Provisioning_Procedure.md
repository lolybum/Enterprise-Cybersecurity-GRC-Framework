# PRC-001 User Account Provisioning Procedure

**Procedure ID:** PRC-001

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
- STD-004 Enterprise Privileged Access Management Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for requesting, approving, creating, modifying, and validating enterprise user accounts to ensure authorized personnel receive appropriate access while protecting organizational information and systems.

This procedure supports the organization's Identity and Access Management (IAM) program by ensuring user accounts are provisioned in accordance with approved business requirements, the principle of least privilege, and applicable security standards.

---

# 2. Scope

This procedure applies to:

- Employees.
- Contractors.
- Temporary workers.
- Consultants.
- Interns.
- Third-party users requiring access.
- Service accounts.
- Application accounts.
- Cloud accounts.
- Remote access accounts.

This procedure applies to all enterprise-managed information systems and applications.

---

# 3. Purpose of the Procedure

This procedure establishes a consistent process for:

- Receiving account requests.
- Verifying authorization.
- Assigning appropriate access.
- Creating user accounts.
- Enforcing authentication controls.
- Enabling Multi-Factor Authentication (MFA).
- Validating successful account creation.
- Documenting provisioning activities.
- Supporting compliance requirements.
- Reducing unauthorized access risk.

---

# 4. Prerequisites

Prior to provisioning a user account, the following shall be completed:

- Approved account request.
- Manager approval.
- Human Resources confirmation for employees.
- Vendor approval for third-party personnel where applicable.
- Completion of required security awareness training where applicable.
- Confirmation of business justification.
- Assignment of appropriate job role.
- Identification of required systems.
- Verification that requested access aligns with least privilege principles.

---

# 5. Roles and Responsibilities

## Requestor

The Requestor shall:

- Submit a completed account request.
- Provide a valid business justification.
- Identify the required systems and applications.
- Ensure the requested access aligns with the user's job responsibilities.

## Hiring Manager

The Hiring Manager shall:

- Approve user account requests.
- Verify the user's employment or contractual relationship.
- Confirm the required access level.
- Ensure the principle of least privilege is applied.

## Human Resources

Human Resources shall:

- Confirm employment status.
- Notify IAM of new hires, transfers, and terminations.
- Maintain employee records supporting account lifecycle activities.

## Identity and Access Management (IAM) Team

The IAM Team shall:

- Review approved requests.
- Provision user accounts.
- Assign access based on approved roles.
- Enforce password and MFA requirements.
- Document provisioning activities.
- Verify successful account creation.

## Information Security Team

The Information Security Team shall:

- Review requests for privileged access where required.
- Validate compliance with security policies.
- Monitor provisioning activities.
- Support security investigations related to user accounts.

---

# 6. Required Tools and Systems

The following enterprise systems may be used during the provisioning process:

- Identity and Access Management (IAM) platform.
- Active Directory or Microsoft Entra ID.
- HR Information System (HRIS).
- ServiceNow or approved IT Service Management (ITSM) platform.
- Multi-Factor Authentication (MFA) platform.
- Privileged Access Management (PAM) solution.
- Enterprise email platform.
- Security Information and Event Management (SIEM) platform.
- Audit logging solution.

Only authorized personnel shall have access to provisioning tools.

---

# 7. User Account Provisioning Workflow

The following workflow shall be followed for all new user account requests.

### Step 1 – Receive Request

- Receive an approved account request through the authorized ITSM system.
- Verify that all required fields are complete.
- Confirm the business justification.
- Confirm manager approval.

---

### Step 2 – Verify Identity

- Confirm the user's identity.
- Verify employment or contractor status.
- Validate onboarding approval from Human Resources where applicable.
- Confirm the user's department and job role.

---

### Step 3 – Determine Required Access

- Identify required applications.
- Determine required network access.
- Identify email requirements.
- Identify shared drive access.
- Identify cloud service access.
- Verify role-based access assignments.
- Apply the Principle of Least Privilege.

---

### Step 4 – Create User Account

- Create the enterprise identity.
- Assign a unique user ID.
- Configure the email account where applicable.
- Assign organizational groups.
- Configure default security settings.
- Apply approved naming conventions.
- Generate an initial temporary password.

---

### Step 5 – Assign Role-Based Access

- Assign approved security groups.
- Assign application roles.
- Assign department-specific access.
- Configure shared resource permissions.
- Verify access inheritance.
- Document all assigned permissions.

Role assignments shall follow approved Role-Based Access Control (RBAC) models.

---

# 8. Access Validation

Following account creation, the IAM Team shall validate that:

- The account was created successfully.
- Required applications are accessible.
- Unauthorized access has not been granted.
- Group memberships are correct.
- Default security settings are applied.
- Audit logging is enabled.
- The account status is active.
- Password policies are enforced.

Any provisioning errors shall be corrected before the account is released to the user.

---

# 9. Multi-Factor Authentication (MFA) Enrollment

Where required by policy:

- Register the user for MFA.
- Verify enrollment completion.
- Validate approved authentication methods.
- Confirm successful MFA authentication.
- Provide user enrollment instructions.
- Document MFA activation.

Users shall complete MFA enrollment before accessing protected enterprise resources unless an approved exception exists.

---

# 10. Documentation Requirements

The following information shall be retained for each provisioning request:

- Request ticket number.
- User name.
- User ID.
- Department.
- Job role.
- Manager approval.
- Systems provisioned.
- Assigned security groups.
- MFA enrollment status.
- Date and time of provisioning.
- IAM administrator performing the work.
- Validation results.

Provisioning records shall be retained in accordance with the organization's records retention requirements.