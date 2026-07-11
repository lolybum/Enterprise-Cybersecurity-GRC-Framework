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

---

# 11. Quality Assurance and Verification

Before a newly provisioned account is released to the user, the IAM Team shall perform a quality assurance review.

Verification activities shall include:

- Confirmation that the approved request matches the provisioned access.
- Verification of user identity.
- Validation of assigned security groups.
- Confirmation of application access.
- Verification of email account functionality.
- Confirmation that password policies have been applied.
- Verification that Multi-Factor Authentication (MFA) is enabled where required.
- Validation that audit logging is operational.
- Confirmation that privileged access has received all required approvals.
- Documentation of verification results.

Accounts failing verification shall not be released until all issues have been corrected.

---

# 12. Exception Handling

Exceptions to this procedure shall follow the Enterprise Exception Management process.

Exception requirements include:

- Documented business justification.
- Risk assessment.
- Identification of compensating security controls.
- Approval from the IAM Manager.
- Approval from the Information Security Team for elevated access.
- Defined expiration date.
- Periodic review of approved exceptions.
- Documentation within the Enterprise Exception Register.

Temporary exceptions shall be removed immediately upon expiration.

---

# 13. Escalation Process

Issues identified during account provisioning shall be escalated according to organizational procedures.

Escalation examples include:

### Level 1 – IAM Administrator

Examples:

- Incomplete requests.
- Missing approvals.
- Provisioning errors.
- Incorrect group assignments.

---

### Level 2 – IAM Manager

Examples:

- Role conflicts.
- Access policy violations.
- High-risk access requests.
- Delayed provisioning affecting business operations.

---

### Level 3 – Information Security Team

Examples:

- Privileged access concerns.
- Segregation of Duties (SoD) conflicts.
- Suspected fraudulent requests.
- Security policy violations.

---

### Level 4 – Chief Information Security Officer (CISO)

Examples:

- Executive access requests requiring exception approval.
- Enterprise-wide provisioning issues.
- Significant security risks.
- Regulatory or audit-related concerns.

All escalations shall be documented within the approved IT Service Management (ITSM) platform.

---

# 14. Audit Logging Requirements

All provisioning activities shall generate audit records sufficient to support security monitoring, investigations, and compliance reviews.

Audit logs shall capture:

- Request identifier.
- User identifier.
- Provisioning administrator.
- Date and time of actions.
- Systems affected.
- Group memberships assigned.
- Privileged access assignments.
- MFA enrollment status.
- Approval records.
- Success or failure of provisioning activities.

Audit logs shall be protected from unauthorized modification and retained in accordance with the Enterprise Security Logging and Monitoring Standard.

---

# 15. Post-Provisioning Activities

Following successful provisioning, the IAM Team shall:

- Notify the requestor and hiring manager.
- Provide onboarding instructions to the user.
- Require password change at first login where applicable.
- Confirm successful user authentication.
- Validate MFA functionality.
- Verify access to required systems.
- Close the provisioning request in the ITSM platform.
- Archive provisioning records.
- Update asset and identity inventories where applicable.
- Monitor for abnormal account activity during the initial access period.

Any issues identified after account activation shall be investigated promptly.

---

# 16. Roles and Responsibilities Matrix

| Role | Responsibilities |
|------|------------------|
| Requestor | Submit complete and accurate access requests with business justification. |
| Hiring Manager | Approve access requests and verify business need. |
| Human Resources | Confirm employment status and notify IAM of onboarding, transfers, and terminations. |
| IAM Administrator | Provision accounts, assign approved access, enforce password and MFA requirements, and document activities. |
| IAM Manager | Oversee provisioning activities, approve exceptions, and resolve escalations. |
| Information Security Team | Review privileged access, monitor compliance, and investigate security concerns. |
| System Owners | Approve application-specific access and validate permissions where required. |
| Internal Audit | Review provisioning processes and verify compliance with policies and standards. |

---

# 17. Compliance

Compliance with this procedure shall be verified through:

- Internal Identity and Access Management (IAM) audits.
- User account provisioning reviews.
- Access control assessments.
- Multi-Factor Authentication (MFA) compliance reviews.
- Segregation of Duties (SoD) assessments.
- Privileged access reviews.
- Regulatory compliance assessments.
- Executive management reviews.
- Independent assurance activities.
- Periodic internal audit testing.

Failure to comply with this procedure may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Temporary suspension of provisioning privileges.
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
- Be reviewed by the Information Security Team where elevated access is requested.
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 19. References

This procedure aligns with:

- NIST SP 800-53 Rev. 5 – Access Control (AC), Identification and Authentication (IA), and Personnel Security (PS) Control Families
- NIST Cybersecurity Framework (CSF) 2.0
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- CIS Controls v8
- Microsoft Identity Security Best Practices
- OWASP Application Security Verification Standard (ASVS) – Authentication Requirements

---

# 20. Related Documents

- GOV-031 Enterprise Identity and Access Management Policy
- STD-001 Enterprise Password Standard
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management Standard
- STD-004 Enterprise Privileged Access Management Standard
- PRC-002 Password Reset Procedure
- PRC-003 Multi-Factor Authentication Enrollment Procedure
- PRC-004 Privileged Access Request Procedure

---

# 21. Records Retention

The following records shall be retained in accordance with the organization's Records Retention Policy:

- User account requests.
- Approval records.
- IAM provisioning logs.
- MFA enrollment records.
- Audit logs.
- Access validation results.
- Exception approvals.
- Escalation records.
- ITSM tickets.
- Provisioning verification checklists.

Retention periods shall comply with applicable legal, regulatory, and contractual requirements.

---

# 22. Procedure Review

This procedure shall be reviewed:

- Annually.
- Following significant IAM technology changes.
- Following major security incidents involving user accounts.
- Following internal or external audit findings.
- Following regulatory or contractual changes.
- Following significant organizational restructuring.

All revisions shall be documented using the organization's document management process.

---

# 23. Approval

| Role | Approval |
|------|----------|
| Chief Information Security Officer | Approved |
| IAM Manager | Approved |
| Information Security Governance Committee | Approved |

---

# 24. Document Control

| Item | Value |
|------|-------|
| Procedure ID | PRC-001 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Procedure Owner | IAM Manager |
| Status | Approved |

---

**End of Procedure**