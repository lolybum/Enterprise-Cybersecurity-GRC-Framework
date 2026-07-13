# PRC-012 Identity and Access Review (Access Recertification) Procedure

**Procedure ID:** PRC-012

**Version:** 1.0

**Owner:** Identity and Access Management (IAM) Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-031 Enterprise Identity and Access Management Policy
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management Standard
- STD-004 Enterprise Privileged Access Management Standard
- STD-018 Enterprise Access Review Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for conducting periodic identity and access reviews to ensure that user access rights remain appropriate, authorized, and aligned with current business responsibilities.

This procedure supports the Principle of Least Privilege, segregation of duties (SoD), regulatory compliance, and the reduction of unauthorized access risks through periodic access recertification.

---

# 2. Scope

This procedure applies to:

- Employee user accounts.
- Contractor accounts.
- Third-party vendor accounts.
- Service accounts.
- Privileged accounts.
- Active Directory accounts.
- Microsoft Entra ID accounts.
- Cloud application accounts.
- Business applications.
- Databases.
- Network devices.
- Security administration platforms.

This procedure applies to all enterprise-managed identities and access privileges.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Verify that user access remains appropriate.
- Remove unnecessary or excessive access.
- Validate privileged account assignments.
- Detect segregation of duties (SoD) conflicts.
- Reduce identity-related security risks.
- Support audit and regulatory compliance.
- Improve identity governance.
- Maintain accurate access records.

---

# 4. Prerequisites

Before initiating an access review, the following shall be completed:

- Current user inventory available.
- Current role definitions documented.
- Asset and application ownership assigned.
- Identity repository synchronized.
- Privileged account inventory available.
- Access review schedule approved.
- Review participants identified.
- IAM reporting tools operational.
- Previous review findings available.

---

# 5. Roles and Responsibilities

## Identity and Access Management (IAM) Team

The IAM Team shall:

- Coordinate enterprise access review campaigns.
- Generate access review reports.
- Validate user access inventories.
- Track review completion.
- Implement approved access changes.
- Maintain access review records.

## Managers

Managers shall:

- Review user access assigned to their direct reports.
- Validate business need for assigned access.
- Approve retention or removal of access.
- Complete reviews within established timelines.
- Escalate discrepancies where appropriate.

## System Owners

System Owners shall:

- Review access to systems under their ownership.
- Validate application-specific permissions.
- Approve or reject access requests.
- Identify excessive privileges.
- Participate in remediation activities.

## Information Security Team

The Information Security Team shall:

- Review privileged access assignments.
- Validate segregation of duties (SoD).
- Monitor completion of access reviews.
- Approve access review exceptions.
- Escalate unresolved risks.

## Internal Audit

Internal Audit may:

- Review completed access certifications.
- Validate compliance with regulatory requirements.
- Assess effectiveness of access review controls.
- Recommend corrective actions.

---

# 6. Access Review Scheduling

Identity and access reviews shall be conducted according to the approved enterprise review schedule.

Minimum review frequencies include:

| Access Type | Review Frequency |
|-------------|-----------------|
| Privileged Accounts | Quarterly |
| High-Risk Applications | Quarterly |
| Financial Systems | Quarterly |
| Standard User Accounts | Semi-Annually |
| Service Accounts | Semi-Annually |
| Third-Party Accounts | Quarterly |
| Cloud Administrative Accounts | Quarterly |
| Emergency (Break-Glass) Accounts | After each use and Quarterly |

Additional reviews may be initiated following:

- Employee transfers.
- Employee termination.
- Organizational restructuring.
- Security incidents.
- Regulatory requirements.
- Management request.

---

# 7. User Access Inventory

Prior to each review, the IAM Team shall generate a complete user access inventory.

The inventory shall include:

- User identifier.
- Employee name.
- Department.
- Manager.
- Employment status.
- Assigned roles.
- Group memberships.
- Privileged access assignments.
- Multi-Factor Authentication (MFA) status.
- Last login date.
- Account status.
- Assigned applications.
- Access approval history.

The inventory shall be validated before distribution to reviewers.

---

# 8. Manager Review Process

Managers shall review access assigned to personnel under their supervision.

The review shall verify:

- Continued employment.
- Current job responsibilities.
- Business justification for access.
- Least Privilege compliance.
- Unused accounts.
- Dormant accounts.
- Shared account usage.
- Temporary access assignments.
- Separation of duties requirements.
- Excessive permissions.

Managers shall select one of the following actions:

- Retain Access
- Modify Access
- Remove Access
- Escalate for Investigation

All decisions shall be documented within the enterprise Identity Governance platform or approved IT Service Management (ITSM) system.

---

# 9. Privileged Access Recertification

Privileged accounts shall undergo enhanced review.

The review shall verify:

- Current business need.
- Administrative responsibilities.
- Multi-Factor Authentication (MFA) compliance.
- Privileged Access Management (PAM) enrollment.
- Emergency account usage.
- Administrative group membership.
- Just-in-Time (JIT) access usage where applicable.
- Administrative activity logs.
- Compliance with the Principle of Least Privilege.

Privileged access that is no longer required shall be removed immediately following approval.

---

# 10. Segregation of Duties (SoD) Validation

Access reviews shall include validation of Segregation of Duties (SoD).

Validation activities include:

- Identify conflicting roles.
- Review incompatible permissions.
- Evaluate financial approval conflicts.
- Review administrative privilege combinations.
- Assess compensating controls.
- Document identified SoD conflicts.
- Escalate unresolved conflicts.
- Approve compensating controls where necessary.

Confirmed SoD violations shall be remediated in accordance with the Enterprise Identity and Access Management Standard.

---

# 11. Access Removal Workflow

Access identified as unnecessary, excessive, or unauthorized during the review process shall be removed promptly.

Access removal activities include:

- Validate the review decision.
- Obtain required approvals.
- Submit an access removal request through the approved Identity Governance or IT Service Management (ITSM) platform.
- Remove unnecessary role assignments.
- Remove group memberships.
- Remove privileged access where applicable.
- Disable dormant accounts where required.
- Verify successful access removal.
- Notify the affected manager and system owner.
- Document all access removal activities.

Access removal shall be completed in accordance with the organization's defined service level objectives (SLOs).

---

# 12. Exception Management

Where access cannot be removed immediately due to operational or business requirements, an exception shall be requested.

Exception requests shall include:

- Business justification.
- User information.
- Systems affected.
- Roles involved.
- Risk assessment.
- Compensating security controls.
- Risk owner approval.
- Information Security approval.
- Exception expiration date.
- Planned remediation date.

Approved exceptions shall be reviewed periodically and maintained within the Enterprise Exception Register.

---

# 13. Audit Evidence Collection

Evidence supporting each access review shall be retained for audit purposes.

Evidence shall include:

- Access review reports.
- User access inventories.
- Manager review decisions.
- System Owner approvals.
- Privileged access review records.
- Segregation of Duties (SoD) assessments.
- Access removal confirmations.
- Exception approvals.
- Executive summary reports.
- Completion records.

Evidence shall be protected from unauthorized modification and retained according to the organization's Records Retention Policy.

---

# 14. Reporting and Metrics

The IAM Team shall prepare periodic reports to evaluate the effectiveness of the access review program.

Reports shall include:

- Review completion percentage.
- Number of users reviewed.
- Number of privileged accounts reviewed.
- Number of access removals.
- Outstanding review tasks.
- Number of Segregation of Duties (SoD) conflicts identified.
- Number of approved exceptions.
- Average review completion time.
- Overdue reviews.
- Trend analysis.

Reports shall be distributed to executive management, Information Security, Internal Audit, and System Owners.

---

# 15. Review Completion and Closure

An access review shall be considered complete only after:

- All assigned reviews have been completed.
- All required approvals have been obtained.
- Approved access removals have been implemented.
- Outstanding exceptions have been documented.
- Review evidence has been retained.
- Reports have been generated.
- Executive summaries have been distributed where required.
- Findings have been documented.
- Corrective actions have been assigned where applicable.

Completed reviews shall be archived according to the organization's Records Retention Policy.

---

# 16. Documentation Requirements

The following records shall be maintained:

- Access review schedules.
- User access inventories.
- Review assignments.
- Manager review records.
- System Owner approvals.
- Privileged access review reports.
- Segregation of Duties (SoD) assessments.
- Access removal records.
- Exception approvals.
- Audit evidence.
- Executive reports.
- Change Management records where applicable.

Documentation shall be retained in accordance with the organization's Records Retention Policy and applicable legal, regulatory, and contractual requirements.

---

# 17. Compliance

Compliance with this procedure shall be verified through:

- Internal Identity and Access Management (IAM) audits.
- Enterprise access certification reviews.
- Privileged access recertification assessments.
- Segregation of Duties (SoD) compliance reviews.
- Regulatory compliance assessments.
- Executive management reviews.
- Independent assurance activities.
- Internal audit testing.
- Continuous compliance monitoring.
- Identity governance maturity assessments.

Failure to comply with this procedure may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Immediate removal of unauthorized access.
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
- Be approved by the Identity and Access Management (IAM) Manager.
- Be reviewed by the Information Security Team.
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 19. References

This procedure aligns with:

- NIST SP 800-53 Rev. 5 – Access Control (AC) and Identification and Authentication (IA) Control Families
- NIST SP 800-63B – Digital Identity Guidelines
- NIST Cybersecurity Framework (CSF) 2.0
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- CIS Controls v8
- ISACA Identity Governance Best Practices
- COBIT 2019 Governance Framework

---

# 20. Related Documents

- GOV-031 Enterprise Identity and Access Management Policy
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management Standard
- STD-004 Enterprise Privileged Access Management Standard
- STD-018 Enterprise Access Review Standard
- PRC-001 User Account Provisioning Procedure
- PRC-002 Password Reset Procedure
- PRC-003 Multi-Factor Authentication (MFA) Enrollment Procedure
- PRC-004 Privileged Access Request Procedure

---

# 21. Procedure Review

This procedure shall be reviewed:

- Annually.
- Following significant changes to IAM technologies.
- Following identity-related security incidents.
- Following audit findings.
- Following regulatory or contractual changes.
- Following significant organizational restructuring.

All revisions shall be documented using the organization's document management process.

---

# 22. Approval

| Role | Approval |
|------|----------|
| Chief Information Security Officer | Approved |
| Identity and Access Management (IAM) Manager | Approved |
| Information Security Governance Committee | Approved |

---

# 23. Document Control

| Item | Value |
|------|-------|
| Procedure ID | PRC-012 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Procedure Owner | Identity and Access Management (IAM) Manager |
| Status | Approved |

---

**End of Procedure**