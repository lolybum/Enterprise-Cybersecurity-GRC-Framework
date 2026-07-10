# STD-007 Enterprise Linux Server Hardening Standard

**Document ID:** STD-007

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-024 Enterprise Security Architecture Policy
- GOV-025 Enterprise Endpoint Security Policy
- GOV-029 Enterprise Vulnerability Management Policy
- GOV-030 Enterprise Patch Management Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Linux Server Hardening Standard is to establish mandatory security configuration requirements for Linux servers deployed across the enterprise.

This standard defines the minimum hardening controls required to reduce attack surfaces, strengthen operating system security, protect enterprise workloads, and support regulatory compliance through standardized Linux security baselines.

---

# 2. Scope

This standard applies to:

- Enterprise Linux servers.
- Red Hat Enterprise Linux (RHEL).
- Rocky Linux.
- AlmaLinux.
- Ubuntu Server.
- Debian Server.
- SUSE Linux Enterprise Server (SLES).
- Cloud-hosted Linux servers.
- Virtual Linux servers.
- Container host operating systems.
- Development, testing, staging, production, and disaster recovery environments.

This standard applies to all Linux server systems owned, operated, or managed by the organization.

---

# 3. Objectives

The objectives of this standard are to:

- Establish secure Linux server baselines.
- Reduce operating system attack surfaces.
- Standardize Linux security configurations.
- Protect enterprise services.
- Support Zero Trust Architecture.
- Improve regulatory compliance.
- Strengthen identity security.
- Improve audit readiness.
- Detect configuration drift.
- Improve enterprise cyber resilience.

---

# 4. Standard Statement

All Linux servers shall be deployed, configured, maintained, and monitored using approved enterprise hardening baselines.

Linux server configurations shall align with:

- CIS Linux Benchmarks.
- NIST SP 800-53 Rev. 5.
- NIST SP 800-123.
- ISO/IEC 27001:2022.
- ISO/IEC 27002:2022.
- Vendor security guidance.
- Organizational security requirements.

Unsupported Linux distributions shall not be deployed in production unless formally approved through the Enterprise Exception Management process.

---

# 5. Linux Installation Requirements

Linux servers shall be deployed using approved enterprise installation images and standardized build procedures.

Installation requirements include:

- Use only organization-approved Linux distributions and supported versions.
- Deploy minimal operating system installations.
- Remove unnecessary packages and services before production deployment.
- Configure secure hostname naming conventions.
- Synchronize system time using approved Network Time Protocol (NTP) services.
- Enable Secure Boot where supported.
- Verify operating system integrity prior to production deployment.
- Document installed packages and system roles.

Only authorized Information Technology personnel may deploy Linux servers.

---

# 6. Operating System Hardening

All Linux servers shall be hardened before deployment into production environments.

Hardening requirements include:

- Remove unnecessary software packages.
- Disable unused services and daemons.
- Disable insecure network protocols.
- Configure secure kernel parameters.
- Enable automatic security updates where approved.
- Configure secure DNS settings.
- Disable unnecessary boot services.
- Protect system configuration files.
- Harden cron and scheduled task configurations.
- Apply approved enterprise hardening baselines.

Linux hardening shall align with CIS Benchmarks and approved vendor guidance.

---

# 7. User and Group Security

User and group management shall follow enterprise Identity and Access Management (IAM) requirements.

Requirements include:

- Assign unique user accounts.
- Prohibit shared administrative accounts.
- Enforce least privilege.
- Disable inactive accounts.
- Remove unused accounts promptly.
- Restrict membership of privileged groups.
- Require Multi-Factor Authentication (MFA) where supported.
- Review user and group memberships periodically.

Administrative accounts shall comply with enterprise IAM and PAM standards.

---

# 8. Secure Shell (SSH) Hardening

SSH shall be securely configured before administrative remote access is permitted.

SSH requirements include:

- Disable direct root login.
- Use SSH protocol version 2 only.
- Require strong cryptographic algorithms.
- Disable weak ciphers and legacy protocols.
- Restrict SSH access using firewall rules.
- Configure session timeout values.
- Limit failed authentication attempts.
- Enable detailed SSH logging.
- Restrict SSH access to authorized administrators.
- Use key-based authentication where approved.

SSH configuration files shall be protected from unauthorized modification.

---

# 9. sudo Configuration

Administrative privilege escalation shall be managed using secure `sudo` configuration.

Requirements include:

- Grant sudo privileges only to authorized personnel.
- Assign privileges based on least privilege.
- Require user authentication before privilege escalation.
- Log all sudo activity.
- Review sudo privileges periodically.
- Remove unnecessary sudo permissions.
- Prohibit unrestricted administrative access.
- Maintain documented sudo role assignments.

Changes to sudo configuration shall follow the Enterprise Change Management process.

---

# 10. File System Permissions

Linux file systems shall be configured to prevent unauthorized access to operating system files and sensitive information.

Requirements include:

- Restrict permissions on system configuration files.
- Secure ownership of operating system directories.
- Protect authentication files such as `/etc/passwd` and `/etc/shadow`.
- Restrict write access to critical system files.
- Configure secure permissions for application data.
- Protect log directories.
- Restrict temporary directory misuse.
- Review file permissions periodically.

File system permissions shall follow the principle of least privilege.

---

# 11. SELinux and AppArmor

Mandatory Access Control (MAC) technologies shall be enabled where supported.

Requirements include:

- Enable SELinux in Enforcing mode on supported distributions.
- Configure AppArmor on supported systems where SELinux is unavailable.
- Maintain approved security policies.
- Monitor policy violations.
- Document approved policy exceptions.
- Review security policies periodically.
- Protect security policy configuration files.
- Integrate policy monitoring with enterprise logging systems.

Disabling SELinux or AppArmor requires documented approval through the Enterprise Exception Management process.

---

# 12. Linux Firewall Configuration

Enterprise Linux servers shall use approved host-based firewall solutions.

Firewall requirements include:

- Enable firewalld, nftables, or another approved firewall technology.
- Block inbound traffic by default unless explicitly authorized.
- Permit only approved services and ports.
- Log firewall events.
- Remove obsolete firewall rules.
- Restrict administrative management ports.
- Review firewall configurations periodically.
- Document firewall exceptions.

Firewall configurations shall align with the Enterprise Network Security Standard.

---

# 13. Patch Management

Linux servers shall be maintained with current security updates to reduce exposure to known vulnerabilities.

Patch management requirements include:

- Deploy operating system security updates in accordance with the Enterprise Patch Management Policy.
- Apply Critical and High severity security patches within organization-defined service level objectives (SLOs).
- Test updates in non-production environments before deployment where appropriate.
- Validate successful installation of patches.
- Remove unsupported software packages.
- Monitor patch compliance across all Linux servers.
- Maintain documented maintenance windows.
- Track and remediate failed patch deployments.

Emergency security updates shall follow the organization's Emergency Change Management process.

---

# 14. Audit Logging

Linux servers shall generate audit logs sufficient to support security monitoring, forensic investigations, and regulatory compliance.

Audit logging requirements include:

- User authentication events.
- Failed login attempts.
- SSH authentication events.
- sudo activity.
- Privileged command execution.
- User account creation and deletion.
- File permission changes.
- Configuration modifications.
- Service start and stop events.
- Kernel and system events.

Where applicable, Linux Audit Framework (auditd) shall be enabled and configured to record security-relevant events.

Audit logs shall be forwarded to the organization's centralized Security Information and Event Management (SIEM) platform.

---

# 15. System Monitoring

Linux servers shall be continuously monitored for security, performance, and operational health.

Monitoring requirements include:

- CPU utilization.
- Memory utilization.
- Disk utilization.
- Service availability.
- System uptime.
- Authentication failures.
- Security events.
- File integrity monitoring.
- Configuration changes.
- Malware detection events where applicable.

Critical security alerts shall be investigated promptly by the Security Operations Center (SOC).

---

# 16. Backup and Recovery

Linux servers shall support secure backup and recovery operations.

Requirements include:

- Scheduled backups of critical systems.
- Encryption of backup data.
- Secure storage of backup media.
- Periodic restoration testing.
- Verification of backup integrity.
- Monitoring of backup success and failures.
- Retention of backups according to enterprise policy.
- Protection of backup repositories from unauthorized access.

Backup configurations shall align with the Enterprise Backup and Recovery Policy.

---

# 17. Malware Protection

Where supported and appropriate, Linux servers shall implement enterprise-approved malware detection and endpoint security solutions.

Requirements include:

- Approved anti-malware or Endpoint Detection and Response (EDR) solution.
- Scheduled malware scans where applicable.
- Real-time monitoring of suspicious activity.
- Signature and detection rule updates.
- Continuous integration with centralized monitoring platforms.
- Investigation of detected threats.
- Isolation of compromised systems where necessary.
- Documentation of malware-related incidents.

Linux malware protection shall be integrated into the organization's incident response process.

---

# 18. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve Linux server security baseline requirements.
- Review Linux server security risks.
- Ensure compliance with applicable regulations and security frameworks.

## Information Security Team

The Information Security Team shall:

- Develop and maintain Linux hardening baselines.
- Monitor compliance with security configuration requirements.
- Conduct security assessments.
- Review security exceptions.
- Recommend improvements to Linux server security controls.

## Information Technology Team

The Information Technology Team shall:

- Deploy Linux servers using approved secure baseline configurations.
- Apply security updates and configuration changes.
- Configure logging, monitoring, and endpoint protection.
- Perform routine compliance checks.
- Remediate identified configuration deficiencies.

## System Owners

System Owners shall:

- Ensure Linux servers remain compliant with this standard.
- Support vulnerability remediation.
- Approve business-related configuration changes.
- Participate in periodic compliance reviews.

## Linux Administrators

Linux Administrators shall:

- Follow approved hardening procedures.
- Use privileged accounts only for authorized administrative tasks.
- Protect administrative credentials.
- Report security incidents promptly.
- Comply with enterprise change management requirements.

---

# 19. Compliance

Compliance with this standard shall be verified through:

- Internal security audits.
- External security assessments.
- Linux configuration compliance reviews.
- CIS Benchmark compliance assessments.
- Vulnerability assessments.
- Penetration testing where applicable.
- Continuous configuration monitoring.
- Regulatory compliance assessments.
- Management reviews.
- Independent assurance activities.

Failure to comply with this standard may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Increased security monitoring.
- Suspension of non-compliant systems from production where necessary.
- Disciplinary action in accordance with organizational policies.
- Contractual action for third parties where applicable.

---

# 20. Exceptions

Exceptions to this standard shall:

- Be formally documented.
- Include a valid business justification.
- Include a documented risk assessment.
- Identify compensating security controls.
- Be approved by the Chief Information Security Officer (CISO).
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 21. References

This standard aligns with:

- NIST SP 800-53 Rev. 5 – Security and Privacy Controls for Information Systems and Organizations
- NIST SP 800-123 – Guide to General Server Security
- NIST Cybersecurity Framework (CSF) 2.0
- NIST SP 800-207 – Zero Trust Architecture
- CIS Benchmarks for Linux
- CIS Controls v8
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- Red Hat Enterprise Linux Security Guide
- Ubuntu Security Documentation
- SUSE Linux Enterprise Security Guide

---

# 22. Related Documents

- GOV-024 Enterprise Security Architecture Policy
- GOV-025 Enterprise Endpoint Security Policy
- GOV-029 Enterprise Vulnerability Management Policy
- GOV-030 Enterprise Patch Management Policy
- GOV-036 Enterprise Backup and Recovery Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-049 Enterprise Zero Trust Architecture Policy
- STD-001 Enterprise Password Standard
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-005 Enterprise Secure Configuration Baseline Standard
- STD-006 Enterprise Windows Server Hardening Standard

---

# 23. Definitions

**Linux Server Hardening** – The process of securely configuring Linux operating systems to reduce vulnerabilities and strengthen system security.

**CIS Benchmark** – A consensus-based secure configuration guideline published by the Center for Internet Security (CIS).

**Secure Shell (SSH)** – A cryptographic network protocol used for secure remote administration of Linux systems.

**SELinux** – Security-Enhanced Linux, a Mandatory Access Control (MAC) security architecture that enforces security policies on Linux systems.

**AppArmor** – A Linux security module that restricts program capabilities using security profiles.

**auditd** – The Linux Audit Framework daemon used to collect and monitor security-relevant events.

**Configuration Drift** – Any unauthorized or unintended deviation from an approved security configuration baseline.

---

# 24. Approval

| Role | Approval |
|------|----------|
| Executive Management | Approved |
| Chief Information Security Officer | Approved |
| Information Security Governance Committee | Approved |

---

# 25. Document Control

| Item | Value |
|------|-------|
| Document ID | STD-007 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Standard Owner | Chief Information Security Officer |
| Status | Approved |

---

**End of Document**