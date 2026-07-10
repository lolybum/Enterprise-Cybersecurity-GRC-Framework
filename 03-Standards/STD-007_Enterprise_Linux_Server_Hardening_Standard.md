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