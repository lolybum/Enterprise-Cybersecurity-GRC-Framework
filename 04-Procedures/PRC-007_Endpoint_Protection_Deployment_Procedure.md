# PRC-007 Endpoint Protection Deployment Procedure

**Procedure ID:** PRC-007

**Version:** 1.0

**Owner:** Endpoint Security Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-024 Enterprise Security Architecture Policy
- STD-005 Enterprise Secure Configuration Baseline Standard
- STD-008 Enterprise Endpoint Protection Standard
- STD-009 Enterprise Network Security Standard
- STD-012 Enterprise Security Logging and Monitoring Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for deploying, configuring, validating, and maintaining enterprise endpoint protection solutions to safeguard organizational devices against malware, ransomware, unauthorized access, and other cybersecurity threats.

This procedure ensures that all enterprise-managed endpoints receive consistent security protection and comply with organizational security requirements before being placed into production.

---

# 2. Scope

This procedure applies to:

- Windows workstations.
- Windows laptops.
- Windows servers.
- Linux endpoints where supported.
- macOS endpoints.
- Virtual desktop infrastructure (VDI).
- Corporate mobile devices where supported.
- Remote workforce endpoints.
- Cloud-managed endpoints.

This procedure applies to all enterprise-owned and managed endpoint devices.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Deploy approved endpoint protection software.
- Protect endpoints against malware and ransomware.
- Enable Endpoint Detection and Response (EDR).
- Strengthen endpoint security posture.
- Standardize endpoint protection deployments.
- Improve threat detection capabilities.
- Support security monitoring.
- Support regulatory compliance.
- Reduce endpoint-related cyber risks.

---

# 4. Prerequisites

Before deploying endpoint protection, the following shall be completed:

- Approved endpoint build.
- Asset registration completed.
- Endpoint ownership assigned.
- Approved operating system installed.
- Network connectivity verified.
- Administrative deployment privileges available.
- Required software licenses assigned.
- Latest endpoint protection software available.
- Change Management approval obtained where required.

---

# 5. Roles and Responsibilities

## Endpoint Security Team

The Endpoint Security Team shall:

- Deploy approved endpoint protection software.
- Configure Endpoint Detection and Response (EDR).
- Maintain endpoint security policies.
- Monitor endpoint protection health.
- Investigate endpoint security alerts.
- Coordinate remediation activities.

## Infrastructure Team

The Infrastructure Team shall:

- Prepare endpoints for deployment.
- Install approved operating systems.
- Verify network connectivity.
- Support software deployment activities.
- Resolve operating system configuration issues.

## Information Security Team

The Information Security Team shall:

- Define endpoint security requirements.
- Review endpoint protection compliance.
- Validate security configurations.
- Approve endpoint protection exceptions.
- Monitor enterprise endpoint risk.

## System Owners

System Owners shall:

- Ensure endpoints remain compliant.
- Coordinate maintenance windows.
- Support remediation activities.
- Report security issues affecting managed endpoints.

---

# 6. Endpoint Onboarding

All enterprise-managed endpoints shall be onboarded into the approved endpoint protection platform before being placed into production.

Onboarding activities include:

- Verify endpoint asset registration.
- Confirm endpoint ownership.
- Validate operating system compatibility.
- Install the approved endpoint protection agent.
- Register the endpoint with the centralized management console.
- Confirm policy synchronization.
- Verify successful communication with the management platform.
- Document onboarding completion.

Endpoints shall not be released for production use until onboarding has been successfully completed.

---

# 7. Endpoint Detection and Response (EDR) Deployment

The approved EDR solution shall be deployed to all supported endpoints.

Deployment requirements include:

- Install the EDR agent.
- Enable behavioral threat detection.
- Enable ransomware protection.
- Enable exploit prevention.
- Enable memory protection.
- Enable real-time telemetry collection.
- Configure automatic policy updates.
- Configure alert forwarding to the SIEM platform.
- Verify successful agent registration.
- Confirm endpoint health status.

EDR agents shall remain enabled at all times unless an approved exception exists.

---

# 8. Anti-Malware Configuration

Enterprise anti-malware protections shall be configured according to approved security baselines.

Configuration requirements include:

- Enable real-time protection.
- Enable scheduled malware scans.
- Enable automatic signature updates.
- Enable cloud-assisted threat intelligence where approved.
- Configure quarantine actions.
- Configure automatic remediation where appropriate.
- Enable archive file scanning.
- Enable removable media scanning.
- Configure scan exclusions only when approved.
- Log malware detection events.

Anti-malware configurations shall be reviewed periodically to ensure continued effectiveness.

---

# 9. Endpoint Firewall Configuration

Host-based firewalls shall be enabled on all enterprise-managed endpoints.

Configuration requirements include:

- Enable firewall protection for all network profiles.
- Block unauthorized inbound connections.
- Restrict outbound connections where appropriate.
- Allow only approved applications and services.
- Remove unused firewall rules.
- Enable firewall logging.
- Forward firewall events to the SIEM platform.
- Review firewall rules periodically.
- Document approved firewall exceptions.

Firewall configurations shall comply with the Enterprise Network Security Standard.

---

# 10. Device Control and USB Security

Endpoint device control shall be configured to reduce the risk of unauthorized data transfer and malware infection.

Configuration requirements include:

- Restrict unauthorized USB storage devices.
- Control external storage device usage.
- Monitor removable media activity.
- Block unauthorized hardware devices where supported.
- Enable device control logging.
- Configure approved device allowlists.
- Encrypt approved removable media where required.
- Review device control policies regularly.
- Investigate unauthorized device connection events.

Device control settings shall support the organization's Data Loss Prevention (DLP) and Endpoint Protection requirements.

---

# 11. Security Policy Assignment

Enterprise endpoint protection policies shall be assigned according to device type, business function, and organizational risk.

Policy assignment requirements include:

- Assign the approved endpoint security policy.
- Apply role-based endpoint security configurations.
- Configure policy inheritance where applicable.
- Verify successful policy synchronization.
- Restrict unauthorized policy modifications.
- Validate endpoint policy version.
- Review policy assignments periodically.
- Document approved policy exceptions.

Endpoints shall not operate without an assigned enterprise security policy.

---

# 12. Compliance Validation

Each endpoint shall undergo compliance validation following deployment.

Validation activities include:

- Confirm endpoint protection agent installation.
- Verify Endpoint Detection and Response (EDR) functionality.
- Validate anti-malware protection.
- Verify firewall configuration.
- Confirm device control policy enforcement.
- Verify endpoint encryption where required.
- Validate operating system patch level.
- Confirm communication with the management console.
- Verify policy synchronization.
- Review endpoint compliance status.

Endpoints failing validation shall not be released to production until deficiencies have been corrected.

---

# 13. Logging and Monitoring

Endpoint protection platforms shall generate security logs to support monitoring, investigations, and compliance.

Logging requirements include:

- Malware detection events.
- Ransomware detection events.
- Endpoint isolation events.
- Policy modification events.
- Firewall events.
- Device control events.
- USB connection events.
- EDR detection events.
- Administrative actions.
- Agent health status.

Security logs shall be forwarded to the enterprise Security Information and Event Management (SIEM) platform and protected against unauthorized modification.

---

# 14. Threat Detection and Response

The Endpoint Security Team shall investigate and respond to endpoint security events.

Response activities include:

- Review endpoint security alerts.
- Validate detected threats.
- Isolate compromised endpoints where necessary.
- Perform malware eradication.
- Coordinate incident response activities.
- Restore endpoints following remediation.
- Conduct post-incident reviews.
- Update detection rules based on lessons learned.
- Document response activities.
- Escalate significant incidents according to the Enterprise Security Incident Response Procedure.

High-risk endpoint security events shall be handled in accordance with the Enterprise Security Incident Response Plan.

---

# 15. Validation and Compliance Checks

Following deployment, each endpoint shall undergo a security validation process.

Validation requirements include:

- Verify endpoint registration.
- Validate EDR functionality.
- Confirm malware protection status.
- Validate firewall configuration.
- Confirm device control enforcement.
- Verify policy assignment.
- Confirm successful communication with the management console.
- Perform vulnerability assessment where required.
- Review security logs.
- Document validation results.

Endpoints that fail validation shall be remediated before production use.

---

# 16. Documentation Requirements

The following records shall be maintained for each protected endpoint:

- Endpoint asset identifier.
- Device owner.
- Operating system version.
- Endpoint protection software version.
- EDR status.
- Anti-malware status.
- Firewall configuration summary.
- Device control policy.
- Compliance validation results.
- Vulnerability assessment results where applicable.
- Exception approvals.
- Change Management records.

Documentation shall be retained in accordance with the organization's Records Retention Policy.