# STD-005 Enterprise Secure Configuration Baseline Standard

**Document ID:** STD-005

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-024 Enterprise Security Architecture Policy
- GOV-025 Enterprise Endpoint Security Policy
- GOV-026 Enterprise Network Security Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Secure Configuration Baseline Standard is to establish mandatory configuration requirements for enterprise systems, operating systems, cloud resources, applications, network devices, and security technologies.

This standard defines the minimum secure configuration controls required to reduce attack surfaces, eliminate insecure default settings, strengthen system resilience, and support the organization's Zero Trust Architecture.

---

# 2. Scope

This standard applies to:

- Windows servers.
- Linux servers.
- Workstations.
- Laptops.
- Mobile devices.
- Cloud platforms.
- Virtual machines.
- Containers.
- Network devices.
- Firewalls.
- Routers.
- Switches.
- Wireless infrastructure.
- Enterprise applications.
- Security appliances.

This standard applies to all production, development, testing, and disaster recovery environments owned or managed by the organization.

---

# 3. Objectives

The objectives of this standard are to:

- Establish secure baseline configurations.
- Reduce system vulnerabilities.
- Eliminate insecure default settings.
- Standardize enterprise configurations.
- Support Zero Trust Architecture.
- Improve system resilience.
- Strengthen regulatory compliance.
- Support automated configuration management.
- Detect configuration drift.
- Improve enterprise security posture.

---

# 4. Standard Statement

The organization shall establish, document, implement, and maintain secure configuration baselines for all enterprise technology assets.

Baseline configurations shall be developed using recognized industry guidance such as CIS Benchmarks, vendor security recommendations, and applicable regulatory requirements.

Configuration baselines shall be reviewed regularly, tested before deployment, and updated following significant technology, security, or regulatory changes.

Unauthorized configuration changes are prohibited unless approved through the Enterprise Change Management process.

---

# 5. Secure Configuration Governance

The organization shall establish governance processes to ensure secure configuration baselines are consistently implemented, maintained, and monitored.

Governance requirements include:

- Approved secure configuration baselines.
- Configuration ownership.
- Baseline documentation.
- Configuration change approval.
- Configuration compliance reviews.
- Configuration risk assessments.
- Periodic baseline updates.
- Executive oversight.

Configuration baselines shall be reviewed at least annually or following significant technology, security, or regulatory changes.

---

# 6. Operating System Baselines

Secure baseline configurations shall be established for all supported operating systems.

Operating system baseline requirements include:

- Removal or disabling of unnecessary services.
- Removal of default accounts where appropriate.
- Secure password policies.
- Multi-Factor Authentication (MFA) integration where supported.
- Host-based firewall configuration.
- Endpoint protection software.
- Secure audit logging.
- Time synchronization.
- Security patch compliance.
- Secure boot configuration where supported.

Operating system baselines shall align with approved CIS Benchmarks or vendor security guidance.

---

# 7. Server Configuration Baselines

Enterprise servers shall be configured using standardized secure baseline configurations.

Server baseline requirements include:

- Minimal operating system installation.
- Removal of unnecessary software.
- Secure administrative access.
- Encryption of sensitive data.
- Secure network services.
- Logging and monitoring.
- Anti-malware protection where applicable.
- Backup configuration.
- Secure remote administration.
- Compliance with enterprise hardening standards.

Production, development, testing, and disaster recovery servers shall each have documented baseline configurations.

---

# 8. Workstation Configuration Baselines

Enterprise workstations shall comply with approved secure configuration baselines.

Workstation requirements include:

- Approved operating system image.
- Endpoint Detection and Response (EDR).
- Host firewall enabled.
- Automatic security updates.
- Disk encryption.
- Screen lock configuration.
- Removal of unauthorized software.
- Secure browser configuration.
- Device compliance monitoring.
- Restricted local administrator privileges.

Workstations shall be regularly assessed for compliance with approved baselines.

---

# 9. Network Device Baselines

Enterprise network infrastructure shall be configured using approved security baselines.

Network device requirements include:

- Secure administrative access.
- Multi-Factor Authentication (MFA) where supported.
- Secure management protocols (SSH, HTTPS).
- Disabled insecure protocols.
- Configuration backups.
- Logging to centralized systems.
- Network segmentation.
- Access control lists (ACLs).
- Time synchronization.
- Configuration integrity monitoring.

Network device configurations shall be reviewed periodically.

---

# 10. Cloud Resource Baselines

Cloud resources shall be deployed using approved secure configuration baselines.

Cloud baseline requirements include:

- Identity and Access Management (IAM) integration.
- Least privilege permissions.
- Encryption at rest.
- Encryption in transit.
- Secure logging.
- Resource tagging.
- Network security groups.
- Secure storage configuration.
- Continuous compliance monitoring.
- Automated configuration validation.

Cloud baseline configurations shall align with enterprise cloud security standards and provider security best practices.