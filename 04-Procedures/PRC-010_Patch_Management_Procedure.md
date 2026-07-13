# PRC-010 Patch Management Procedure

**Procedure ID:** PRC-010

**Version:** 1.0

**Owner:** Patch Management Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-026 Enterprise Patch Management Policy
- STD-011 Enterprise Patch Management Standard
- STD-012 Enterprise Security Logging and Monitoring Standard
- STD-020 Enterprise Business Continuity and Disaster Recovery Standard
- STD-023 Enterprise Vulnerability Scanning Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for identifying, evaluating, testing, approving, deploying, validating, and documenting security patches across enterprise information systems.

This procedure ensures security patches are implemented in a timely and controlled manner to reduce cybersecurity risk while minimizing operational disruption.

---

# 2. Scope

This procedure applies to:

- Windows servers.
- Linux servers.
- Workstations.
- Laptops.
- Network devices.
- Firewalls.
- Databases.
- Virtual machines.
- Cloud-hosted systems.
- Security appliances.
- Third-party software.

This procedure applies to all enterprise-managed technology assets.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Identify newly released security patches.
- Prioritize patch deployment based on business risk.
- Reduce exposure to known vulnerabilities.
- Validate successful patch installation.
- Support regulatory compliance.
- Improve system resilience.
- Standardize patch deployment activities.
- Minimize service disruption.

---

# 4. Prerequisites

Before initiating patch management activities, the following shall be completed:

- Asset inventory is current.
- Asset ownership has been assigned.
- Approved maintenance windows exist.
- Backup procedures have been completed where required.
- Vulnerability scan results are available.
- Patch repositories are operational.
- Change Management procedures are available.
- Rollback procedures have been documented.
- Business stakeholders have been notified where required.

---

# 5. Roles and Responsibilities

## Patch Management Team

The Patch Management Team shall:

- Monitor vendor security advisories.
- Coordinate enterprise patch deployment activities.
- Maintain the enterprise patch management platform.
- Validate patch deployment success.
- Produce patch compliance reports.
- Coordinate emergency patching activities.

## Infrastructure Team

The Infrastructure Team shall:

- Deploy operating system patches.
- Deploy firmware updates where applicable.
- Validate system functionality after patching.
- Resolve patch installation failures.
- Participate in rollback activities when required.

## Application Owners

The Application Owners shall:

- Evaluate application compatibility.
- Test application functionality following patch installation.
- Coordinate application maintenance windows.
- Approve application-specific deployment schedules.

## Information Security Team

The Information Security Team shall:

- Assess patch-related security risks.
- Prioritize security patches.
- Review emergency patch requests.
- Validate compliance with enterprise security standards.
- Monitor remediation timelines.

## Change Advisory Board (CAB)

The Change Advisory Board shall:

- Review significant patch deployments.
- Evaluate operational risks.
- Approve production implementation.
- Review emergency changes after implementation.

---

# 6. Patch Identification

Security patches shall be identified through approved information sources.

Patch sources include:

- Operating system vendors.
- Application vendors.
- Security appliance vendors.
- Vendor security bulletins.
- Vulnerability scan results.
- Threat intelligence services.
- National Vulnerability Database (NVD).
- Common Vulnerabilities and Exposures (CVE) notifications.
- Cybersecurity advisories issued by applicable government agencies.

Patch information shall be reviewed on a scheduled basis.

---

# 7. Patch Risk Classification

Patches shall be prioritized according to enterprise risk.

Classification factors include:

- CVSS severity score.
- Vendor severity rating.
- Exploit availability.
- Asset criticality.
- Internet exposure.
- Business impact.
- Regulatory requirements.
- Existing compensating controls.
- Threat intelligence.

Enterprise patch priorities shall be classified as:

| Priority | Description |
|----------|-------------|
| Critical | Immediate deployment required |
| High | Expedited deployment required |
| Medium | Scheduled deployment |
| Low | Routine maintenance deployment |

Patch priorities may be adjusted based on business risk.

---

# 8. Patch Testing

Patches shall be tested before production deployment whenever practical.

Testing activities include:

- Install patches within a test environment.
- Verify operating system functionality.
- Verify application compatibility.
- Validate security controls.
- Confirm service availability.
- Identify deployment issues.
- Evaluate rollback procedures.
- Document test results.
- Obtain testing approval.

Emergency security patches may follow an expedited testing process when approved.

---

# 9. Patch Approval Workflow

Patch deployment shall follow the enterprise Change Management process.

Approval workflow includes:

- Patch identification.
- Risk assessment.
- Testing completion.
- Technical review.
- Information Security review.
- Business approval where required.
- Change Advisory Board (CAB) approval for significant deployments.
- Deployment authorization.

No production patch deployment shall occur without the required approvals unless emergency procedures apply.

---

# 10. Deployment Scheduling

Patch deployment shall occur during approved maintenance windows whenever possible.

Scheduling requirements include:

- Coordinate with business stakeholders.
- Notify affected users.
- Verify backup completion.
- Confirm rollback readiness.
- Schedule deployment according to patch priority.
- Coordinate with Infrastructure and Application teams.
- Validate resource availability.
- Minimize business disruption.
- Document deployment schedules.

Emergency security patches shall be deployed as soon as operationally feasible following approval.