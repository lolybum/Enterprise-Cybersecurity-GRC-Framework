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