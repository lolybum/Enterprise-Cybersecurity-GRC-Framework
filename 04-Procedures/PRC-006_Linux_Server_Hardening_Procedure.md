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