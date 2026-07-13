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

---

# 11. SIEM Correlation Rules

The SIEM platform shall use correlation rules to identify malicious activity by analyzing events from multiple log sources.

Correlation rule requirements include:

- Detect brute-force authentication attacks.
- Detect impossible travel events.
- Detect privileged account misuse.
- Detect excessive failed login attempts.
- Detect suspicious PowerShell activity.
- Detect privilege escalation events.
- Detect lateral movement techniques.
- Detect malware execution.
- Detect ransomware indicators.
- Detect data exfiltration attempts.
- Detect unauthorized configuration changes.
- Detect command-and-control (C2) communications.
- Detect known Indicators of Compromise (IOCs).
- Detect insider threat indicators.
- Detect policy violations.

Correlation rules shall be reviewed quarterly and updated based on emerging threats, threat intelligence, and lessons learned from security incidents.

---

# 12. Security Alert Triage

All SIEM-generated alerts shall undergo triage by the Security Operations Center (SOC).

Triage activities include:

- Validate alert accuracy.
- Identify false positives.
- Determine event severity.
- Assess business impact.
- Determine affected assets.
- Review associated logs.
- Correlate related security events.
- Assign incident priority.
- Document investigation findings.
- Escalate confirmed security incidents.

Alert priorities shall follow the Enterprise Incident Severity Matrix.

---

# 13. Incident Escalation

Confirmed security incidents shall be escalated in accordance with the Enterprise Security Incident Response Procedure.

Escalation workflow includes:

### Level 1 – SOC Analyst

Responsibilities include:

- Initial alert review.
- Event validation.
- Basic investigation.
- False positive identification.
- Documentation.

---

### Level 2 – Senior SOC Analyst

Responsibilities include:

- Advanced investigation.
- Threat correlation.
- Malware analysis.
- Threat hunting.
- Initial containment recommendations.

---

### Level 3 – Incident Response Team

Responsibilities include:

- Incident containment.
- Eradication activities.
- Forensic evidence collection.
- Recovery coordination.
- Executive reporting.

---

### Level 4 – Chief Information Security Officer (CISO)

Responsibilities include:

- Executive decision-making.
- Regulatory notification oversight.
- Business risk communication.
- Coordination with executive leadership.
- External stakeholder communication where required.

All escalation activities shall be documented within the approved incident management platform.

---

# 14. Dashboard and Reporting

The SIEM platform shall provide operational and executive dashboards.

Dashboards shall include:

- Security alerts by severity.
- Open security incidents.
- Mean Time to Detect (MTTD).
- Mean Time to Respond (MTTR).
- Log ingestion status.
- Endpoint Detection and Response (EDR) events.
- Authentication failures.
- Threat intelligence matches.
- Firewall events.
- Vulnerability trends.
- Compliance monitoring results.
- Executive risk summaries.

Reports shall be distributed according to approved reporting schedules.

---

# 15. Continuous Monitoring

The SOC shall continuously monitor enterprise security events.

Continuous monitoring activities include:

- Review SIEM dashboards.
- Investigate new alerts.
- Monitor threat intelligence feeds.
- Review endpoint security events.
- Monitor privileged account activity.
- Monitor firewall events.
- Monitor cloud security alerts.
- Review system health.
- Verify log ingestion status.
- Escalate significant findings.

Monitoring shall operate 24x7 where required by business or regulatory requirements.

---

# 16. Documentation Requirements

The following records shall be maintained:

- SIEM onboarding documentation.
- Log source inventory.
- Correlation rule documentation.
- Alert configuration records.
- Alert investigation records.
- Incident escalation records.
- Dashboard reports.
- Executive reports.
- Threat hunting documentation.
- Log retention records.
- Audit logs.
- Change Management records.

Documentation shall be retained in accordance with the organization's Records Retention Policy and applicable legal, regulatory, and contractual requirements.

---

# 17. Compliance

Compliance with this procedure shall be verified through:

- Internal Information Security audits.
- Security Operations Center (SOC) operational assessments.
- SIEM health and performance reviews.
- Log source onboarding validation.
- Security alert effectiveness reviews.
- Regulatory compliance assessments.
- Executive management reviews.
- Independent assurance activities.
- Internal audit testing.
- Continuous monitoring maturity assessments.

Failure to comply with this procedure may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Increased management oversight.
- Temporary suspension of non-compliant log sources.
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
- Be approved by the SOC Manager.
- Be reviewed by the Information Security Team.
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 19. References

This procedure aligns with:

- NIST SP 800-92 – Guide to Computer Security Log Management
- NIST SP 800-53 Rev. 5 – Security and Privacy Controls for Information Systems and Organizations
- NIST Cybersecurity Framework (CSF) 2.0
- MITRE ATT&CK Framework
- CIS Controls v8
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- ISO/IEC 27035 – Information Security Incident Management
- SANS Critical Security Controls

---

# 20. Related Documents

- GOV-027 Enterprise Security Monitoring Policy
- STD-012 Enterprise Security Logging and Monitoring Standard
- STD-019 Enterprise Security Incident Response Standard
- STD-022 Enterprise Security Configuration Compliance Monitoring Standard
- STD-025 Enterprise Security Operations Center (SOC) Operations Standard
- PRC-008 Firewall Rule Change Management Procedure
- PRC-009 Vulnerability Management Procedure
- PRC-019 Security Incident Response Procedure

---

# 21. Procedure Review

This procedure shall be reviewed:

- Annually.
- Following significant SIEM platform upgrades.
- Following major security incidents.
- Following audit findings.
- Following regulatory or contractual changes.
- Following significant changes to enterprise monitoring architecture.

All revisions shall be documented using the organization's document management process.

---

# 22. Approval

| Role | Approval |
|------|----------|
| Chief Information Security Officer | Approved |
| Security Operations Center (SOC) Manager | Approved |
| Information Security Governance Committee | Approved |

---

# 23. Document Control

| Item | Value |
|------|-------|
| Procedure ID | PRC-011 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Procedure Owner | Security Operations Center (SOC) Manager |
| Status | Approved |

---

**End of Procedure**