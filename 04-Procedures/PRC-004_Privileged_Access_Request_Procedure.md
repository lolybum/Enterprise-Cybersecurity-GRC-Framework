# PRC-004 Privileged Access Request Procedure

**Procedure ID:** PRC-004

**Version:** 1.0

**Owner:** Privileged Access Management (PAM) Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-031 Enterprise Identity and Access Management Policy
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management Standard
- STD-004 Enterprise Privileged Access Management Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for requesting, approving, provisioning, monitoring, and revoking privileged access to enterprise systems.

This procedure ensures privileged access is granted only to authorized personnel with a validated business need, appropriate approvals, and appropriate security controls.

---

# 2. Scope

This procedure applies to:

- Domain administrators.
- Server administrators.
- Database administrators.
- Network administrators.
- Cloud administrators.
- Security administrators.
- Application administrators.
- DevOps engineers.
- Third-party administrators.
- Emergency ("break-glass") privileged accounts.

This procedure applies to all privileged accounts used to administer enterprise-managed systems, applications, cloud services, and network infrastructure.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Ensure privileged access is properly authorized.
- Enforce the Principle of Least Privilege.
- Support Just-in-Time (JIT) privileged access where available.
- Enforce Multi-Factor Authentication (MFA).
- Maintain complete audit records.
- Reduce the risk of unauthorized privileged access.
- Support regulatory and audit requirements.
- Standardize privileged access management processes across the enterprise.

---

# 4. Prerequisites

Prior to requesting privileged access, the following requirements shall be met:

- The requester has an active enterprise account.
- Identity verification has been completed.
- Required security awareness training has been completed.
- A documented business justification exists.
- Manager approval has been obtained.
- The requested privileged role has been identified.
- A valid IT Service Management (ITSM) request has been submitted.
- The requester agrees to comply with enterprise privileged access requirements.

---

# 5. Roles and Responsibilities

## Requestor

The Requestor shall:

- Submit a privileged access request through the approved IT Service Management (ITSM) platform.
- Provide a valid business justification.
- Complete all required security awareness training.
- Use privileged access only for authorized business purposes.
- Comply with enterprise security policies and standards.

## Manager

The Manager shall:

- Review the business justification.
- Confirm the business need.
- Verify that the requested access aligns with the user's job responsibilities.
- Approve or reject the request.

## System Owner

The System Owner shall:

- Review requests affecting systems under their responsibility.
- Validate the requested privilege level.
- Ensure the Principle of Least Privilege is applied.
- Approve or reject system-specific privileged access.

## Privileged Access Management (PAM) Team

The PAM Team shall:

- Review approved requests.
- Provision privileged accounts.
- Configure Just-in-Time (JIT) access where available.
- Enforce Multi-Factor Authentication (MFA).
- Configure session monitoring where applicable.
- Document provisioning activities.

## Information Security Team

The Information Security Team shall:

- Review high-risk privileged access requests.
- Assess Segregation of Duties (SoD) conflicts.
- Review exception requests.
- Monitor privileged account activity.
- Investigate suspicious privileged activity.

---

# 6. Privileged Access Request Workflow

### Step 1 – Submit Request

The Requestor shall:

- Submit an ITSM request.
- Identify the required privileged role.
- Provide a business justification.
- Specify requested systems.
- Specify the requested duration of access.

---

### Step 2 – Manager Approval

The Manager shall:

- Validate the business requirement.
- Confirm the requester's job responsibilities.
- Verify the requested duration.
- Approve or reject the request.

---

### Step 3 – System Owner Approval

Where applicable, the System Owner shall:

- Review requested privileges.
- Validate least privilege.
- Confirm the requester requires administrative access.
- Approve or reject the request.

---

### Step 4 – Information Security Review

For high-risk or privileged roles, Information Security shall:

- Review the request.
- Evaluate Segregation of Duties (SoD).
- Assess security risks.
- Recommend additional controls where appropriate.
- Approve or reject elevated requests.

---

### Step 5 – PAM Provisioning

Following approval, the PAM Team shall:

- Create or assign the privileged account.
- Configure approved permissions.
- Apply role-based access controls.
- Enable session logging.
- Enable privileged session monitoring.
- Require Multi-Factor Authentication (MFA).
- Document provisioning activities.

---

# 7. Approval Requirements

Privileged access shall not be granted without the required approvals.

Minimum approval requirements include:

- Requestor submission.
- Manager approval.
- System Owner approval where applicable.
- Information Security approval for elevated privileges.
- PAM Team validation prior to provisioning.

Emergency access approvals shall follow the Break-Glass Access process.

---

# 8. Privileged Access Provisioning

The PAM Team shall ensure that:

- Privileged accounts use unique credentials.
- Shared administrator accounts are prohibited unless specifically approved.
- Password vaulting is implemented where supported.
- MFA is enforced.
- Session recording is enabled where supported.
- Administrative privileges are assigned only to approved users.
- Default administrative accounts are secured.
- Audit logging is enabled.

Provisioning activities shall be documented within the ITSM platform.

---

# 9. Just-in-Time (JIT) Privileged Access

Where supported, privileged access shall be granted using Just-in-Time (JIT) principles.

JIT requirements include:

- Time-limited privileged access.
- Automatic privilege expiration.
- Workflow-based approval.
- Session monitoring.
- Automatic session termination after expiration.
- Complete audit logging.

Standing privileged access shall be minimized whenever technically feasible.

---

# 10. Emergency (Break-Glass) Access

Emergency privileged access shall only be used when normal administrative access is unavailable or immediate action is required to restore critical business operations.

Break-Glass requirements include:

- Executive or Incident Manager authorization.
- Immediate notification to the Information Security Team.
- Time-limited privileged access.
- Continuous monitoring of all activities.
- Mandatory post-event review.
- Immediate removal of emergency privileges after use.
- Documentation of all emergency activities.

All Break-Glass events shall be reviewed as part of the organization's post-incident review process.

---

# 11. Privileged Session Monitoring

All privileged sessions shall be monitored to ensure authorized use and support security investigations.

Monitoring requirements include:

- Session recording where technically supported.
- Real-time monitoring of high-risk privileged sessions.
- Logging of authentication events.
- Logging of privileged commands where supported.
- Monitoring of privileged account activity.
- Detection of anomalous privileged behavior.
- Alert generation for suspicious activities.
- Secure retention of session logs.
- Protection of monitoring records from unauthorized modification.
- Periodic review of privileged session logs.

Monitoring data shall be retained in accordance with the Enterprise Security Logging and Monitoring Standard.

---

# 12. Access Review and Recertification

Privileged access shall be reviewed regularly to ensure continued business need.

Review requirements include:

- Quarterly privileged access reviews.
- Manager validation of continued business need.
- System Owner review of assigned privileges.
- Information Security review of privileged roles.
- Removal of unnecessary privileges.
- Validation of Segregation of Duties (SoD).
- Review of inactive privileged accounts.
- Documentation of review results.
- Tracking of corrective actions.

Access that is no longer required shall be revoked immediately.

---

# 13. Privileged Access Revocation

Privileged access shall be removed promptly when it is no longer required.

Revocation shall occur following:

- Employee termination.
- Role change.
- Transfer to another department.
- Completion of temporary assignments.
- Expiration of Just-in-Time (JIT) access.
- Completion of emergency (Break-Glass) access.
- Discovery of unauthorized privileged activity.
- Information Security direction.

Following revocation, the PAM Team shall:

- Remove privileged group memberships.
- Disable privileged accounts where appropriate.
- Remove privileged credentials from password vaults.
- Terminate active privileged sessions.
- Verify successful removal of access.
- Document all revocation activities.

---

# 14. Audit Logging Requirements

All privileged access activities shall generate audit records.

Audit logs shall include:

- Request identifier.
- User identifier.
- Privileged role assigned.
- Systems affected.
- Approval records.
- Provisioning date and time.
- Session start and end times.
- Administrative actions performed.
- Privileged access revocation activities.
- Break-Glass access activities.
- Exception approvals.
- Escalation records.

Audit logs shall be retained and protected in accordance with the Enterprise Security Logging and Monitoring Standard.

---

# 15. Exception Handling

Exceptions to this procedure shall follow the Enterprise Exception Management process.

Exception requirements include:

- Documented business justification.
- Risk assessment.
- Identification of compensating security controls.
- Approval by the PAM Manager.
- Information Security review.
- Defined expiration date.
- Periodic review of approved exceptions.
- Documentation within the Enterprise Exception Register.

Temporary exceptions shall be removed immediately upon expiration.

---

# 16. Escalation Process

Issues involving privileged access shall be escalated according to organizational procedures.

### Level 1 – PAM Administrator

Examples:

- Standard provisioning requests.
- Group membership updates.
- Password vault synchronization issues.
- Routine administrative support.

---

### Level 2 – PAM Manager

Examples:

- High-risk privileged access requests.
- Delayed provisioning.
- Access conflicts.
- Policy interpretation issues.

---

### Level 3 – Information Security Team

Examples:

- Segregation of Duties (SoD) conflicts.
- Unauthorized privileged activity.
- Privileged account compromise.
- Security policy violations.

---

### Level 4 – Chief Information Security Officer (CISO)

Examples:

- Executive privileged access exceptions.
- Enterprise-wide privileged access issues.
- Regulatory or audit concerns.
- Significant cybersecurity incidents involving privileged accounts.

All escalations shall be documented within the approved IT Service Management (ITSM) platform.