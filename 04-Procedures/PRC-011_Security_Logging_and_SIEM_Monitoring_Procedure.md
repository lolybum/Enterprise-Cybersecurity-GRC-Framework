# PRC-011 Security Logging and SIEM Monitoring Procedure

**Procedure ID:** PRC-011

**Version:** 1.0

**Owner:** Security Operations Center (SOC) Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-027 Enterprise Security Monitoring Policy
- STD-012 Enterprise Security Logging and Monitoring Standard
- STD-019 Enterprise Security Incident Response Standard
- STD-022 Enterprise Security Configuration Compliance Monitoring Standard
- STD-025 Enterprise Security Operations Center (SOC) Operations Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for collecting, protecting, monitoring, analyzing, and retaining security logs using the enterprise Security Information and Event Management (SIEM) platform.

This procedure ensures security events are detected, investigated, escalated, and documented in a timely manner while supporting regulatory, legal, and operational requirements.

---

# 2. Scope

This procedure applies to:

- Windows servers.
- Linux servers.
- Active Directory.
- Microsoft Entra ID.
- Firewalls.
- Routers and switches.
- Endpoint Detection and Response (EDR) platforms.
- Identity and Access Management (IAM) systems.
- Cloud platforms.
- Databases.
- Web applications.
- Security appliances.
- SIEM infrastructure.

This procedure applies to all enterprise-managed log sources.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Centralize enterprise security logging.
- Improve threat detection capabilities.
- Support Security Operations Center (SOC) monitoring.
- Enable rapid incident detection.
- Support forensic investigations.
- Improve regulatory compliance.
- Support audit activities.
- Maintain complete security event records.
- Strengthen enterprise security visibility.

---

# 4. Prerequisites

Before security logging activities begin, the following shall be completed:

- SIEM platform deployed.
- Approved log retention policy.
- Approved log source inventory.
- Network connectivity verified.
- Time synchronization configured.
- Logging standards implemented.
- Security alerting configured.
- Incident response contacts available.
- Change Management approval completed where applicable.

---

# 5. Roles and Responsibilities

## Security Operations Center (SOC) Team

The SOC Team shall:

- Monitor the enterprise SIEM platform.
- Review and triage security alerts.
- Investigate suspicious events.
- Escalate confirmed security incidents.
- Maintain monitoring dashboards.
- Document all investigation activities.

## SIEM Administration Team

The SIEM Administration Team shall:

- Maintain the SIEM infrastructure.
- Onboard approved log sources.
- Configure log parsers and normalization rules.
- Maintain correlation rules.
- Optimize SIEM performance.
- Maintain log storage capacity.

## Information Security Team

The Information Security Team shall:

- Define logging requirements.
- Approve monitoring use cases.
- Review detection rules.
- Validate compliance with enterprise security standards.
- Approve logging exceptions.
- Conduct periodic logging assessments.

## System Owners

System Owners shall:

- Ensure systems generate required logs.
- Support log source onboarding.
- Validate application logging.
- Coordinate remediation activities.
- Notify the SOC Team of significant system changes.

## Incident Response Team

The Incident Response Team shall:

- Respond to escalated security incidents.
- Coordinate containment activities.
- Conduct forensic investigations.
- Document incident response actions.
- Support post-incident reviews.

---

# 6. Log Source Onboarding

All enterprise-managed systems shall be onboarded into the approved SIEM platform.

Log onboarding activities include:

- Identify the log source.
- Verify business ownership.
- Configure secure log forwarding.
- Validate connectivity to the SIEM platform.
- Verify event parsing.
- Validate timestamp synchronization.
- Assign log source classification.
- Document onboarding completion.

Only approved log sources shall transmit logs to the enterprise SIEM platform.

---

# 7. Log Collection and Normalization

The SIEM platform shall collect and normalize security logs from approved sources.

Collection requirements include:

- Collect security events in near real time.
- Normalize log formats.
- Standardize timestamps.
- Preserve original event data.
- Identify event source.
- Categorize event severity.
- Eliminate duplicate events where appropriate.
- Validate successful log ingestion.
- Monitor collection health.

Log normalization shall support enterprise reporting, alerting, investigations, and threat hunting.

---

# 8. SIEM Integration

Enterprise security technologies shall integrate with the SIEM platform.

Supported integrations include:

- Microsoft Active Directory.
- Microsoft Entra ID.
- Endpoint Detection and Response (EDR).
- Firewalls.
- Intrusion Detection and Prevention Systems (IDS/IPS).
- Vulnerability Management platforms.
- Identity and Access Management (IAM) solutions.
- Cloud platforms.
- Web application firewalls.
- Email security platforms.

All integrations shall be validated before production use.

---

# 9. Log Retention and Protection

Security logs shall be protected against unauthorized access, modification, or deletion.

Retention requirements include:

- Encrypt logs in transit.
- Encrypt logs at rest.
- Restrict access using Role-Based Access Control (RBAC).
- Protect log integrity.
- Maintain immutable storage where supported.
- Archive logs according to retention requirements.
- Perform periodic integrity validation.
- Secure backup copies of logs.
- Dispose of logs securely after the retention period expires.

Log retention periods shall comply with legal, regulatory, contractual, and business requirements.

---

# 10. Security Alert Configuration

The SIEM platform shall generate alerts for approved security use cases.

Alert configuration requirements include:

- Authentication failures.
- Privileged account activity.
- Account lockouts.
- Malware detections.
- Endpoint Detection and Response (EDR) alerts.
- Firewall policy violations.
- Unauthorized configuration changes.
- Suspicious PowerShell activity.
- Data exfiltration indicators.
- Threat intelligence matches.
- Lateral movement indicators.
- Command and Control (C2) communications.

Alert thresholds shall be reviewed periodically to reduce false positives and improve detection accuracy.