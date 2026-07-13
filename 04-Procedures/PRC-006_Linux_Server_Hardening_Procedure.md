# PRC-006 Linux Server Hardening Procedure

**Procedure ID:** PRC-006

**Version:** 1.0

**Owner:** Infrastructure Security Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-024 Enterprise Security Architecture Policy
- STD-005 Enterprise Secure Configuration Baseline Standard
- STD-007 Enterprise Linux Server Hardening Standard
- STD-008 Enterprise Endpoint Protection Standard
- STD-009 Enterprise Network Security Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for securely configuring, hardening, validating, and maintaining Linux servers to reduce cybersecurity risk and improve the security posture of enterprise infrastructure.

This procedure ensures Linux servers are deployed using approved security baselines, hardened before production use, and maintained throughout their operational lifecycle.

---

# 2. Scope

This procedure applies to:

- Ubuntu Server
- Red Hat Enterprise Linux (RHEL)
- Rocky Linux
- AlmaLinux
- Oracle Linux
- Debian Linux
- SUSE Linux Enterprise Server (SLES)
- Physical Linux servers
- Virtual Linux servers
- Cloud-hosted Linux servers

This procedure applies to all enterprise-managed Linux server environments.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Implement approved Linux security baselines.
- Reduce the Linux attack surface.
- Strengthen authentication and authorization controls.
- Secure privileged accounts.
- Improve system logging and monitoring.
- Protect network communications.
- Support regulatory compliance.
- Standardize Linux server deployments.
- Support continuous security improvement.

---

# 4. Prerequisites

Before beginning Linux server hardening activities, the following shall be completed:

- Approved server build request.
- Approved Linux distribution and version.
- Asset registration completed.
- Server ownership assigned.
- Network configuration completed.
- Required security software available.
- Latest operating system updates available.
- Backup completed before implementing hardening changes.
- Change Management approval obtained.

---

# 5. Roles and Responsibilities

## Infrastructure Team

The Infrastructure Team shall:

- Build Linux server systems.
- Install the approved Linux distribution.
- Configure baseline settings.
- Apply approved security configurations.
- Coordinate with the Information Security Team.
- Document all hardening activities.

## Information Security Team

The Information Security Team shall:

- Maintain approved Linux hardening baselines.
- Validate compliance with security standards.
- Perform security reviews.
- Conduct configuration assessments.
- Approve security exceptions.
- Monitor compliance.

## System Owner

The System Owner shall:

- Approve server deployment.
- Validate business requirements.
- Coordinate maintenance windows.
- Review security recommendations.
- Support remediation activities.

## Change Management

The Change Management Team shall:

- Review change requests.
- Approve production implementation.
- Maintain change records.
- Verify successful implementation.

---

# 6. Linux Server Build Preparation

Before hardening begins, verify the Linux server has been built according to enterprise standards.

Preparation activities include:

- Install the approved Linux distribution and version.
- Apply the latest supported operating system updates.
- Verify the server hostname.
- Configure static IP addressing where required.
- Join enterprise identity services where applicable.
- Synchronize system time using approved NTP servers.
- Verify hardware health.
- Install approved system packages only.
- Register the server within the Configuration Management Database (CMDB).

---

# 7. Operating System Hardening

The Linux operating system shall be configured according to approved enterprise security baselines.

Hardening requirements include:

- Remove unnecessary packages.
- Remove unused services.
- Disable unnecessary daemons.
- Disable unused network protocols.
- Enable automatic security updates where approved.
- Configure Secure Boot where supported.
- Enable full disk encryption where required.
- Configure kernel security parameters (sysctl).
- Disable core dumps where appropriate.
- Restrict access to system utilities.
- Configure approved time synchronization.
- Apply CIS Benchmarks or approved security baselines.

Operating system hardening shall be validated before production deployment.

---

# 8. User and Group Security

User and group management shall follow the Principle of Least Privilege.

Configuration requirements include:

- Disable direct root login where possible.
- Use sudo for privileged administration.
- Remove unnecessary user accounts.
- Remove inactive accounts.
- Configure password aging policies.
- Configure password complexity requirements.
- Lock unused service accounts.
- Restrict membership of privileged groups.
- Review user and group memberships regularly.
- Configure account lockout protections where supported.

Administrative privileges shall only be assigned to authorized personnel.

---

# 9. SSH Hardening

Secure Shell (SSH) shall be configured using enterprise-approved security settings.

Configuration requirements include:

- Disable SSH protocol version 1.
- Disable direct root login.
- Require SSH protocol version 2.
- Use strong cryptographic algorithms.
- Disable password authentication where public key authentication is used.
- Configure idle session timeouts.
- Restrict SSH access using approved user or group lists.
- Enable Multi-Factor Authentication (MFA) where supported.
- Limit login attempts.
- Log SSH authentication events.

SSH configuration shall be validated before production deployment.

---

# 10. Linux Firewall Configuration

An approved host-based firewall shall be enabled on all Linux servers.

Firewall requirements include:

- Enable UFW, firewalld, or iptables/nftables based on the approved Linux distribution.
- Block inbound connections unless explicitly authorized.
- Restrict outbound connections where appropriate.
- Allow only approved service ports.
- Remove unused firewall rules.
- Document approved exceptions.
- Enable firewall logging where appropriate.
- Forward firewall logs to the enterprise logging platform.
- Periodically review firewall rules.
- Verify firewall configuration after system updates.

Firewall configurations shall comply with the Enterprise Network Security Standard.

---

# 11. Package Management and Security Updates

Linux servers shall be maintained using approved package repositories and secure update procedures.

Package management requirements include:

- Configure approved enterprise software repositories.
- Verify package authenticity using cryptographic signatures.
- Remove unsupported or deprecated packages.
- Apply security patches in accordance with the Enterprise Patch Management Standard.
- Test critical updates prior to production deployment where practical.
- Schedule maintenance windows for updates.
- Remove obsolete kernels after validation.
- Verify successful package installation.
- Document failed updates.
- Escalate update failures according to Change Management procedures.

Only trusted repositories approved by the organization shall be used.

---

# 12. Audit Logging Configuration

Linux audit logging shall be configured to support security monitoring, incident response, and compliance requirements.

Configuration requirements include:

- Enable the Linux Audit Framework (auditd).
- Log authentication events.
- Log privilege escalation events.
- Log sudo activities.
- Log user account creation and modification.
- Log changes to critical system files.
- Log service start and stop events.
- Log kernel module loading.
- Log system configuration changes.
- Protect audit logs from unauthorized modification.

Audit logs shall comply with the Enterprise Security Logging and Monitoring Standard.

---

# 13. File System Security

Critical system files and directories shall be protected using approved security controls.

Configuration requirements include:

- Restrict permissions on system configuration files.
- Restrict access to `/etc/passwd` and `/etc/shadow`.
- Protect SSH configuration files.
- Configure appropriate ownership of system directories.
- Enable secure mount options where appropriate.
- Disable execution from temporary directories where feasible.
- Restrict write access to critical system locations.
- Monitor file integrity using approved tools where deployed.
- Encrypt sensitive data where required.
- Periodically review file permissions.

File system permissions shall support the Principle of Least Privilege.

---

# 14. Logging and Monitoring

Linux servers shall forward security logs to the enterprise logging platform.

Logging requirements include:

- Forward system logs to the Security Information and Event Management (SIEM) platform.
- Monitor authentication events.
- Monitor sudo activity.
- Monitor failed login attempts.
- Monitor privilege escalation events.
- Monitor firewall events.
- Monitor SSH activity.
- Monitor service failures.
- Configure alerts for high-risk security events.
- Protect log integrity and confidentiality.

Logs shall be retained in accordance with the Enterprise Security Logging and Monitoring Standard.

---

# 15. Validation and Compliance Checks

Following hardening activities, each Linux server shall undergo validation to confirm compliance with enterprise requirements.

Validation activities include:

- Verify compliance with approved Linux security baselines.
- Perform vulnerability scanning.
- Review user and group configurations.
- Validate SSH configuration.
- Validate firewall configuration.
- Confirm successful installation of security updates.
- Verify audit logging configuration.
- Validate log forwarding to the SIEM platform.
- Review privileged account configuration.
- Confirm removal of unnecessary packages and services.

Servers failing validation shall not be promoted to production until corrective actions have been completed.

---

# 16. Documentation Requirements

The following records shall be maintained for each hardened Linux server:

- Server hostname.
- Asset identifier.
- Linux distribution and version.
- Hardening completion date.
- Security baseline version applied.
- Package update status.
- Firewall configuration summary.
- Audit logging configuration.
- Vulnerability scan results.
- Validation checklist.
- Exception approvals where applicable.
- Change Management records.

Documentation shall be retained in accordance with the organization's Records Retention Policy.

---

# 17. Compliance

Compliance with this procedure shall be verified through:

- Internal Information Security audits.
- Linux server hardening reviews.
- Secure configuration baseline assessments.
- Vulnerability scanning and remediation verification.
- Linux firewall configuration reviews.
- SSH configuration assessments.
- Audit logging and monitoring reviews.
- Regulatory compliance assessments.
- Executive management reviews.
- Independent assurance activities.

Failure to comply with this procedure may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Delayed production deployment.
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
- Be approved by the Infrastructure Security Manager.
- Be reviewed by the Information Security Team.
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 19. References

This procedure aligns with:

- NIST SP 800-53 Rev. 5 – Security and Privacy Controls for Information Systems and Organizations
- NIST SP 800-123 – Guide to General Server Security
- NIST Cybersecurity Framework (CSF) 2.0
- CIS Benchmarks for Linux
- DISA Security Technical Implementation Guides (STIGs)
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- CIS Controls v8

---

# 20. Related Documents

- GOV-024 Enterprise Security Architecture Policy
- STD-005 Enterprise Secure Configuration Baseline Standard
- STD-007 Enterprise Linux Server Hardening Standard
- STD-008 Enterprise Endpoint Protection Standard
- STD-009 Enterprise Network Security Standard
- STD-011 Enterprise Patch Management Standard
- STD-012 Enterprise Security Logging and Monitoring Standard
- PRC-005 Windows Server Hardening Procedure

---

# 21. Procedure Review

This procedure shall be reviewed:

- Annually.
- Following significant Linux operating system releases.
- Following major security incidents affecting Linux servers.
- Following audit findings.
- Following regulatory or contractual changes.
- Following significant infrastructure changes.

All revisions shall be documented using the organization's document management process.

---

# 22. Approval

| Role | Approval |
|------|----------|
| Chief Information Security Officer | Approved |
| Infrastructure Security Manager | Approved |
| Information Security Governance Committee | Approved |

---

# 23. Document Control

| Item | Value |
|------|-------|
| Procedure ID | PRC-006 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Procedure Owner | Infrastructure Security Manager |
| Status | Approved |

---

**End of Procedure**