# STD-025 Enterprise Security Operations Center (SOC) Operations Standard

**Document ID:** STD-025

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-024 Enterprise Security Architecture Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-040 Enterprise Incident Management Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Security Operations Center (SOC) Operations Standard is to establish mandatory requirements for the continuous monitoring, detection, investigation, escalation, and response to cybersecurity events affecting organizational systems, networks, applications, cloud services, and data.

This standard defines the operational requirements for Security Operations Center (SOC) functions, security event management, threat detection, alert triage, incident escalation, case management, and continuous improvement of enterprise security operations.

---

# 2. Scope

This standard applies to:

- Security Operations Center (SOC) personnel.
- Information Security personnel.
- Information Technology personnel.
- Managed Security Service Providers (MSSPs).
- Cloud security operations.
- Endpoint Detection and Response (EDR) platforms.
- Security Information and Event Management (SIEM) platforms.
- Identity services.
- Enterprise applications.
- Network infrastructure.
- Cloud infrastructure.
- Third-party monitoring services where applicable.

This standard applies to all enterprise-managed technology assets that generate security events or require security monitoring.

---

# 3. Objectives

The objectives of this standard are to:

- Continuously monitor enterprise security events.
- Detect malicious activity.
- Reduce Mean Time to Detect (MTTD).
- Reduce Mean Time to Respond (MTTR).
- Improve incident triage.
- Enhance threat visibility.
- Strengthen enterprise cyber resilience.
- Improve operational efficiency.
- Support regulatory compliance.
- Promote continuous improvement of SOC operations.

---

# 4. Standard Statement

The organization shall operate a Security Operations Center (SOC) capable of continuously monitoring enterprise technology assets, detecting cybersecurity threats, analyzing security events, coordinating incident response, and supporting enterprise cyber defense.

SOC operations shall utilize approved technologies, documented procedures, qualified personnel, and risk-based monitoring processes that align with enterprise security objectives and regulatory requirements.

SOC activities shall integrate with logging, threat intelligence, incident response, vulnerability management, and business continuity capabilities.

---

# 5. SOC Governance

The organization shall establish governance processes to ensure Security Operations Center (SOC) activities are effectively managed, monitored, and continuously improved.

SOC governance requirements include:

- Documented SOC operating procedures.
- Defined SOC roles and responsibilities.
- Executive oversight of SOC operations.
- Integration with Enterprise Risk Management (ERM).
- Integration with Incident Response processes.
- Coordination with Vulnerability Management.
- Periodic review of SOC effectiveness.
- Continuous improvement of SOC capabilities.

SOC governance shall be reviewed at least annually or following significant business, regulatory, technology, or threat landscape changes.

---

# 6. Security Event Monitoring

The Security Operations Center (SOC) shall continuously monitor enterprise technology assets for security events that may indicate malicious activity or policy violations.

Monitoring requirements include:

- Endpoint security events.
- Server security events.
- Authentication and identity events.
- Network security events.
- Firewall events.
- Intrusion Detection and Prevention System (IDS/IPS) events.
- Cloud security events.
- Database security events.
- Application security events.
- Data Loss Prevention (DLP) events.

Security event monitoring shall operate continuously where technically feasible.

---

# 7. Security Information and Event Management (SIEM) Operations

Enterprise security events shall be centralized within an approved Security Information and Event Management (SIEM) platform.

SIEM operational requirements include:

- Centralized log collection.
- Secure log transmission.
- Event normalization.
- Event correlation.
- Threat detection rules.
- Alert generation.
- Log retention.
- Time synchronization.
- Secure access controls.
- High availability where required.

SIEM configurations shall be reviewed periodically to ensure continued effectiveness.

---

# 8. Alert Triage and Prioritization

All security alerts shall undergo structured triage to determine severity, business impact, and required response actions.

Alert triage activities include:

- Validation of alerts.
- Identification of false positives.
- Severity classification.
- Business impact assessment.
- Threat intelligence correlation.
- Asset criticality assessment.
- User impact assessment.
- Escalation where appropriate.
- Incident creation where required.
- Documentation of triage decisions.

Alert prioritization shall consider organizational risk, asset criticality, and regulatory obligations.

---

# 9. Threat Intelligence Integration

The SOC shall integrate threat intelligence into monitoring and detection activities.

Threat intelligence requirements include:

- Commercial threat intelligence feeds.
- Open-source threat intelligence.
- Government advisories where applicable.
- Industry Information Sharing and Analysis Centers (ISACs) where applicable.
- Indicators of Compromise (IOCs).
- Indicators of Attack (IOAs).
- Threat actor profiling.
- MITRE ATT&CK mapping.
- Detection rule updates.
- Intelligence-driven threat hunting.

Threat intelligence shall be evaluated regularly for relevance and accuracy.

---

# 10. Detection Engineering

The organization shall establish a Detection Engineering capability to improve the effectiveness of threat detection.

Detection Engineering requirements include:

- Development of detection use cases.
- Creation of SIEM correlation rules.
- Development of Endpoint Detection and Response (EDR) detection logic.
- MITRE ATT&CK technique mapping.
- Threat intelligence integration.
- Detection tuning.
- False positive reduction.
- Detection testing and validation.
- Continuous improvement of detection content.
- Documentation of detection logic.

Detection content shall be reviewed and updated following significant threat intelligence, security incidents, or technology changes.

---

# 11. Threat Hunting

The organization shall maintain a proactive Threat Hunting capability to identify malicious activity that may evade automated detection mechanisms.

Threat hunting requirements include:

- Risk-based threat hunting activities.
- Hypothesis-driven investigations.
- Threat intelligence-informed hunting.
- MITRE ATT&CK technique mapping.
- Endpoint artifact analysis.
- Network traffic analysis.
- Cloud workload investigations.
- Identity and authentication analysis.
- Detection of anomalous user behavior.
- Documentation of threat hunting results.

Threat hunting activities shall be performed on a scheduled basis and following significant threat intelligence or major security incidents.

---

# 12. Endpoint Detection and Response (EDR) Operations

Enterprise-managed endpoints shall be protected using approved Endpoint Detection and Response (EDR) technologies.

EDR operational requirements include:

- Continuous endpoint monitoring.
- Behavioral threat detection.
- Malware detection.
- Ransomware detection.
- Memory-based attack detection.
- Endpoint isolation capabilities.
- Automated response actions where approved.
- Collection of forensic artifacts.
- Detection rule tuning.
- Integration with SIEM and Incident Response processes.

EDR alerts shall be reviewed promptly according to their assigned severity.

---

# 13. Case Management

The Security Operations Center (SOC) shall maintain a formal case management process for security investigations.

Case management requirements include:

- Unique case identification.
- Incident ownership assignment.
- Investigation documentation.
- Evidence collection.
- Timeline reconstruction.
- Threat intelligence correlation.
- Root cause documentation.
- Escalation tracking.
- Remediation tracking.
- Case closure approval.

Case records shall be retained in accordance with organizational record retention requirements.

---

# 14. Escalation Procedures

The organization shall maintain documented escalation procedures to ensure timely response to cybersecurity events.

Escalation requirements include:

- Severity-based escalation criteria.
- Escalation to Incident Response Team.
- Escalation to executive management.
- Escalation to Legal where appropriate.
- Escalation to Human Resources where applicable.
- Third-party notification procedures.
- Regulatory reporting procedures where required.
- Customer notification coordination where applicable.
- Documentation of escalation decisions.
- Post-escalation review.

Escalation procedures shall support rapid containment and recovery while minimizing business impact.

---

# 15. SOC Metrics and Key Performance Indicators (KPIs)

The organization shall establish metrics to evaluate the effectiveness of Security Operations Center (SOC) activities.

SOC metrics shall include:

- Mean Time to Detect (MTTD).
- Mean Time to Respond (MTTR).
- Mean Time to Contain (MTTC).
- Number of security events processed.
- Number of incidents investigated.
- Alert false positive rate.
- Threat hunting activities completed.
- Detection coverage by MITRE ATT&CK techniques.
- Incident escalation rates.
- Executive SOC dashboard reporting.

Metrics shall be reviewed regularly by executive management and the Information Security Governance Committee to support continuous improvement.

---

# 16. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve enterprise SOC operational requirements.
- Review SOC performance metrics.
- Ensure compliance with applicable regulations and security frameworks.

## Security Operations Center (SOC) Manager

The SOC Manager shall:

- Manage day-to-day SOC operations.
- Ensure adequate staffing and coverage.
- Review SOC performance metrics.
- Approve operational procedures.
- Coordinate continuous improvement initiatives.
- Report SOC performance to executive management.

## SOC Analysts

SOC Analysts shall:

- Monitor enterprise security events.
- Triage and investigate security alerts.
- Escalate incidents according to approved procedures.
- Document investigation activities.
- Support threat hunting activities.
- Maintain accurate case records.

## Detection Engineering Team

The Detection Engineering Team shall:

- Develop and maintain detection rules.
- Tune SIEM and EDR detections.
- Reduce false positives.
- Integrate threat intelligence into detection logic.
- Validate detection effectiveness.

## Incident Response Team

The Incident Response Team shall:

- Respond to escalated cybersecurity incidents.
- Coordinate containment, eradication, and recovery.
- Preserve digital evidence.
- Conduct post-incident reviews.
- Recommend improvements to SOC operations.

## Information Technology Team

The Information Technology Team shall:

- Support SOC investigations.
- Maintain logging infrastructure.
- Implement corrective actions.
- Support endpoint isolation and recovery.
- Coordinate system restoration activities.

## System Owners

System Owners shall:

- Support security investigations affecting their systems.
- Review findings related to assigned assets.
- Coordinate remediation activities.
- Participate in post-incident reviews where required.

## Internal Audit

Internal Audit shall:

- Assess compliance with this standard.
- Review SOC governance processes.
- Validate corrective actions.
- Report significant deficiencies to executive management.

## Users

Users shall:

- Report suspected cybersecurity incidents promptly.
- Cooperate with authorized investigations.
- Comply with organizational security policies.
- Refrain from interfering with approved security monitoring activities.