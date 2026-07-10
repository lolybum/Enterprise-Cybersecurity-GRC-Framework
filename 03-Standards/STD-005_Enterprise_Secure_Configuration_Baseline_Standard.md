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

---

# 11. Configuration Compliance Monitoring

The organization shall continuously monitor enterprise technology assets to verify compliance with approved secure configuration baselines.

Configuration compliance monitoring requirements include:

- Automated configuration compliance scanning.
- Continuous monitoring of critical systems.
- Periodic manual configuration reviews where automation is unavailable.
- Compliance dashboards for management reporting.
- Risk-based prioritization of configuration findings.
- Documentation of non-compliant systems.
- Tracking of remediation activities.
- Verification of corrective actions.

Configuration compliance reports shall be reviewed regularly by Information Security and Information Technology management.

---

# 12. Configuration Drift Detection

The organization shall implement mechanisms to detect unauthorized or unintended deviations from approved configuration baselines.

Configuration drift detection requirements include:

- Automated baseline comparison.
- Detection of unauthorized configuration changes.
- Real-time alerts for critical deviations.
- Investigation of configuration drift.
- Validation of authorized changes.
- Documentation of identified deviations.
- Remediation of unauthorized changes.
- Periodic review of configuration drift trends.

Configuration drift shall be investigated promptly to determine potential security risks.

---

# 13. Change Control Integration

Configuration changes shall be managed through the organization's Enterprise Change Management process.

Requirements include:

- Approved change requests prior to implementation.
- Risk assessment of proposed configuration changes.
- Security review for high-risk changes.
- Testing in non-production environments where appropriate.
- Rollback procedures for failed changes.
- Documentation of implemented changes.
- Verification of successful implementation.
- Post-implementation review.

Emergency changes shall follow the organization's emergency change management procedures and be reviewed after implementation.

---

# 14. Baseline Exceptions

Exceptions to approved secure configuration baselines shall be formally managed.

Requirements include:

- Documented business justification.
- Risk assessment.
- Identification of compensating security controls.
- Approval by the Chief Information Security Officer (CISO) or authorized delegate.
- Defined expiration date.
- Periodic review.
- Documentation within the Enterprise Exception Register.
- Removal of the exception when no longer required.

Baseline exceptions shall not become permanent without formal review and approval.

---

# 15. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve enterprise configuration baseline requirements.
- Review configuration-related risks.
- Ensure alignment with applicable regulations and security frameworks.

## Information Security Team

The Information Security Team shall:

- Develop and maintain secure configuration baselines.
- Monitor configuration compliance.
- Conduct configuration security assessments.
- Review configuration exceptions.
- Recommend baseline improvements.

## Information Technology Team

The Information Technology Team shall:

- Implement approved secure configuration baselines.
- Maintain enterprise systems in accordance with baseline requirements.
- Perform configuration updates through approved change management processes.
- Monitor system configuration compliance.
- Remediate identified configuration deviations.

## System Owners

System Owners shall:

- Ensure systems comply with approved configuration baselines.
- Approve system-specific configuration changes.
- Support compliance reviews and remediation activities.
- Maintain system configuration documentation.

## Users

Users shall:

- Refrain from making unauthorized configuration changes.
- Report suspected unauthorized system modifications.
- Comply with organizational security requirements.
- Cooperate with configuration compliance activities.

---

# 16. Compliance

Compliance with this standard shall be verified through:

- Internal security audits.
- External audits.
- Secure configuration baseline assessments.
- Configuration compliance scans.
- Vulnerability assessments.
- Penetration testing where applicable.
- Continuous configuration monitoring.
- Regulatory compliance assessments.
- Management reviews.
- Independent assurance activities.

Failure to comply with this standard may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Suspension of non-compliant systems from production.
- Increased security monitoring.
- Disciplinary action in accordance with organizational policies.
- Contractual action for third parties where applicable.

---

# 17. Exceptions

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

# 18. References

This standard aligns with:

- NIST SP 800-53 Rev. 5
- NIST SP 800-128 – Guide for Security-Focused Configuration Management
- NIST Cybersecurity Framework (CSF) 2.0
- NIST SP 800-207 – Zero Trust Architecture
- CIS Benchmarks
- CIS Controls v8
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- COBIT 2019
- Vendor Security Hardening Guides

---

# 19. Related Documents

- GOV-016 Enterprise Change Management Policy
- GOV-024 Enterprise Security Architecture Policy
- GOV-025 Enterprise Endpoint Security Policy
- GOV-026 Enterprise Network Security Policy
- GOV-049 Enterprise Zero Trust Architecture Policy
- STD-001 Enterprise Password Standard
- STD-002 Enterprise Multi-Factor Authentication Standard
- STD-003 Enterprise Identity and Access Management (IAM) Standard
- STD-004 Enterprise Privileged Access Management (PAM) Standard

---

# 20. Definitions

**Configuration Baseline** – A formally approved set of security configuration settings used as the standard for deploying and maintaining enterprise technology assets.

**Configuration Drift** – Any unauthorized or unintended deviation from an approved secure configuration baseline.

**System Hardening** – The process of reducing a system's attack surface by securely configuring software, services, operating systems, and network settings.

**Configuration Compliance** – The process of verifying that systems remain aligned with approved secure configuration baselines.

**Configuration Management** – The process of establishing, documenting, implementing, monitoring, and maintaining approved configurations throughout a system's lifecycle.

**Compensating Control** – An alternative security control implemented to reduce risk when a standard requirement cannot be fully met.

---

# 21. Approval

| Role | Approval |
|------|----------|
| Executive Management | Approved |
| Chief Information Security Officer | Approved |
| Information Security Governance Committee | Approved |

---

# 22. Document Control

| Item | Value |
|------|-------|
| Document ID | STD-005 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Standard Owner | Chief Information Security Officer |
| Status | Approved |

---

**End of Document**