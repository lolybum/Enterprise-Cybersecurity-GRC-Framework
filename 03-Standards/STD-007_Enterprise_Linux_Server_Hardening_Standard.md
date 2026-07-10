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