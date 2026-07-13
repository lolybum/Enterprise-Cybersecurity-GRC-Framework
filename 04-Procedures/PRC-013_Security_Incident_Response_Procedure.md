# PRC-013 Security Incident Response Procedure

**Procedure ID:** PRC-013

**Version:** 1.0

**Owner:** Security Operations Center (SOC) Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-028 Enterprise Security Incident Management Policy
- STD-012 Enterprise Security Logging and Monitoring Standard
- STD-019 Enterprise Security Incident Response Standard
- STD-020 Enterprise Business Continuity and Disaster Recovery Standard
- STD-025 Enterprise Security Operations Center (SOC) Operations Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for identifying, analyzing, containing, eradicating, recovering from, documenting, and reporting cybersecurity incidents affecting enterprise information systems.

This procedure ensures incidents are managed consistently, efficiently, and in accordance with legal, regulatory, contractual, and business requirements.

---

# 2. Scope

This procedure applies to:

- Security Operations Center (SOC).
- Information Security Team.
- Incident Response Team.
- IT Operations.
- Cloud environments.
- On-premises infrastructure.
- Endpoints.
- Servers.
- Network devices.
- Applications.
- Databases.
- Third-party managed environments where contractually applicable.

This procedure applies to all confirmed or suspected cybersecurity incidents involving enterprise-managed assets.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Detect cybersecurity incidents quickly.
- Minimize business disruption.
- Protect enterprise information assets.
- Preserve forensic evidence.
- Coordinate incident response activities.
- Meet regulatory notification obligations.
- Improve organizational resilience.
- Support continuous improvement through lessons learned.

---

# 4. Prerequisites

Before responding to a security incident, the following shall be available:

- Approved Incident Response Plan.
- Incident Severity Matrix.
- Security contact list.
- Incident Response Team roster.
- Security monitoring tools.
- SIEM platform.
- Endpoint Detection and Response (EDR) platform.
- Digital forensic tools.
- Secure evidence storage.
- Chain of Custody documentation.
- Executive escalation contacts.

---

# 5. Roles and Responsibilities

## Security Operations Center (SOC)

The SOC Team shall:

- Monitor enterprise security alerts.
- Identify potential security incidents.
- Perform initial incident triage.
- Escalate confirmed incidents.
- Document investigation activities.
- Coordinate with the Incident Response Team.

## Incident Response Team

The Incident Response Team shall:

- Lead incident response activities.
- Coordinate containment efforts.
- Preserve digital evidence.
- Conduct forensic investigations.
- Coordinate eradication and recovery activities.
- Produce incident reports.

## Information Security Team

The Information Security Team shall:

- Provide technical guidance.
- Assess incident impact.
- Review regulatory requirements.
- Coordinate with Legal and Compliance.
- Recommend security improvements.
- Review lessons learned.

## IT Operations Team

The IT Operations Team shall:

- Support containment activities.
- Restore affected systems.
- Deploy remediation actions.
- Validate system functionality.
- Assist with infrastructure recovery.

## System Owners

System Owners shall:

- Validate business impact.
- Assist with system recovery.
- Verify application functionality.
- Approve return to production.

## Legal and Compliance

Legal and Compliance shall:

- Assess regulatory notification requirements.
- Coordinate legal communications.
- Support evidence preservation.
- Review contractual obligations.

---

# 6. Incident Identification

Potential cybersecurity incidents may be identified through multiple sources.

Identification sources include:

- SIEM alerts.
- Endpoint Detection and Response (EDR) alerts.
- Firewall alerts.
- Intrusion Detection and Prevention Systems (IDS/IPS).
- Vulnerability Management tools.
- Threat intelligence notifications.
- User reports.
- Third-party notifications.
- Cloud security monitoring.
- Security audits.
- Automated monitoring systems.

Every suspected incident shall be recorded within the approved Incident Management platform.

---

# 7. Incident Classification

Following identification, each incident shall be classified according to its characteristics.

Incident categories include:

- Malware Infection.
- Ransomware.
- Unauthorized Access.
- Data Breach.
- Insider Threat.
- Denial of Service (DoS/DDoS).
- Phishing Attack.
- Business Email Compromise (BEC).
- Credential Compromise.
- Web Application Attack.
- Cloud Security Incident.
- Third-Party Security Incident.
- Physical Security Incident affecting information assets.

Classification shall support consistent incident handling and reporting.

---

# 8. Incident Severity Levels

Incidents shall be assigned a severity level based on business impact, technical impact, and urgency.

| Severity | Description |
|----------|-------------|
| Critical | Enterprise-wide impact, regulatory reporting likely, major business disruption |
| High | Significant business impact requiring immediate response |
| Medium | Limited business impact with manageable operational disruption |
| Low | Minimal business impact with no significant operational disruption |

Severity may be adjusted as additional information becomes available during the investigation.

---

# 9. Incident Triage

The SOC Team shall perform initial triage for every reported incident.

Triage activities include:

- Validate the reported event.
- Determine whether the event is a true security incident.
- Identify affected systems.
- Assess business impact.
- Determine incident severity.
- Review related security alerts.
- Correlate supporting evidence.
- Assign incident ownership.
- Document initial findings.
- Escalate incidents requiring further investigation.

False positives shall be documented and closed according to SOC procedures.

---

# 10. Initial Response Actions

Following incident confirmation, immediate response actions shall be initiated.

Initial response activities include:

- Notify the Incident Response Team.
- Notify system owners.
- Preserve volatile evidence where appropriate.
- Isolate affected systems if necessary.
- Prevent further compromise.
- Secure affected user accounts.
- Initiate incident communications.
- Record all response activities.
- Determine whether regulatory notification may be required.
- Activate the Incident Response Plan where applicable.

All actions shall be documented within the approved Incident Management platform.

---

# 11. Containment Procedures

Following incident confirmation, containment measures shall be implemented to limit the spread and impact of the incident while preserving business operations where possible.

Containment activities include:

- Isolate affected endpoints from the network.
- Block malicious IP addresses and domains.
- Disable compromised user accounts.
- Revoke compromised authentication tokens.
- Block malicious firewall traffic.
- Disable affected services where required.
- Preserve critical business operations whenever possible.
- Monitor for additional malicious activity.
- Document all containment actions.

Containment actions shall be approved by the Incident Response Team Leader when operationally feasible.

---

# 12. Evidence Collection and Chain of Custody

Digital evidence shall be collected and preserved to support investigations, legal proceedings, and regulatory requirements.

Evidence collection activities include:

- Capture volatile memory where appropriate.
- Acquire forensic disk images.
- Collect system and application logs.
- Preserve firewall logs.
- Preserve SIEM alerts.
- Preserve EDR telemetry.
- Collect network packet captures where available.
- Preserve email evidence.
- Record timestamps.
- Secure evidence in approved storage.

Chain of Custody requirements include:

- Assign a unique evidence identifier.
- Record evidence description.
- Record date and time of collection.
- Record collector name.
- Record transfer history.
- Record storage location.
- Restrict evidence access.
- Protect evidence integrity.
- Retain evidence according to legal and regulatory requirements.

Evidence shall remain admissible and protected against unauthorized modification.

---

# 13. Eradication

Following successful containment, the Incident Response Team shall remove the root cause of the incident.

Eradication activities include:

- Remove malware.
- Eliminate persistence mechanisms.
- Remove unauthorized accounts.
- Patch exploited vulnerabilities.
- Reconfigure affected systems.
- Reset compromised credentials.
- Remove malicious scheduled tasks.
- Remove unauthorized software.
- Update endpoint protection signatures.
- Validate eradication success.

Systems shall not proceed to recovery until eradication activities have been completed successfully.

---

# 14. Recovery

Following eradication, affected systems shall be restored to normal business operations.

Recovery activities include:

- Restore systems from approved backups where necessary.
- Reconnect isolated systems.
- Validate operating system functionality.
- Validate application functionality.
- Verify user authentication.
- Verify network connectivity.
- Confirm business service availability.
- Monitor systems for signs of recurring compromise.
- Obtain System Owner approval before returning systems to production.
- Document recovery activities.

Recovery shall occur in accordance with the organization's Business Continuity and Disaster Recovery procedures.

---

# 15. Post-Incident Review

A formal Post-Incident Review (PIR) shall be conducted following closure of significant security incidents.

The review shall include:

- Incident timeline.
- Root cause analysis.
- Incident response effectiveness.
- Communication effectiveness.
- Business impact assessment.
- Regulatory obligations.
- Control effectiveness.
- Improvement opportunities.
- Assigned corrective actions.
- Executive summary.

The Post-Incident Review shall be completed within the organization's defined review timeframe.

---

# 16. Lessons Learned

The Incident Response Team shall conduct a Lessons Learned session following significant incidents.

Lessons learned activities include:

- Identify successful response activities.
- Identify response gaps.
- Review detection effectiveness.
- Review containment effectiveness.
- Review recovery effectiveness.
- Recommend control improvements.
- Update security monitoring use cases.
- Update incident response playbooks.
- Update security awareness training where appropriate.
- Track corrective actions through completion.

Lessons learned shall be incorporated into future incident response planning and continuous improvement initiatives.

---

# 17. Compliance

Compliance with this procedure shall be verified through:

- Internal Information Security audits.
- Security Incident Response program assessments.
- Security Operations Center (SOC) operational reviews.
- Incident response tabletop exercises.
- Digital forensic process reviews.
- Regulatory compliance assessments.
- Executive management reviews.
- Independent assurance activities.
- Internal audit testing.
- Continuous incident response maturity assessments.

Failure to comply with this procedure may result in:

- Corrective action plans.
- Mandatory remediation activities.
- Increased management oversight.
- Escalation to executive leadership.
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
- Be approved by the Incident Response Manager.
- Be reviewed by the Information Security Team.
- Include an expiration date.
- Be reviewed at least annually.

Approved exceptions shall be maintained within the Enterprise Exception Register.

---

# 19. References

This procedure aligns with:

- NIST SP 800-61 Rev. 2 – Computer Security Incident Handling Guide
- NIST SP 800-53 Rev. 5 – Security and Privacy Controls for Information Systems and Organizations
- NIST Cybersecurity Framework (CSF) 2.0
- MITRE ATT&CK Framework
- ISO/IEC 27035 – Information Security Incident Management
- ISO/IEC 27001:2022
- ISO/IEC 27002:2022
- CIS Controls v8
- SANS Incident Handler's Handbook

---

# 20. Related Documents

- GOV-028 Enterprise Security Incident Management Policy
- STD-012 Enterprise Security Logging and Monitoring Standard
- STD-019 Enterprise Security Incident Response Standard
- STD-020 Enterprise Business Continuity and Disaster Recovery Standard
- STD-025 Enterprise Security Operations Center (SOC) Operations Standard
- PRC-009 Vulnerability Management Procedure
- PRC-010 Patch Management Procedure
- PRC-011 Security Logging and SIEM Monitoring Procedure

---

# 21. Procedure Review

This procedure shall be reviewed:

- Annually.
- Following major cybersecurity incidents.
- Following significant changes to incident response technologies.
- Following audit findings.
- Following regulatory or contractual changes.
- Following updates to the Enterprise Incident Response Plan.

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
| Procedure ID | PRC-013 |
| Version | 1.0 |
| Effective Date | July 2026 |
| Review Cycle | Annual |
| Classification | Internal |
| Procedure Owner | Security Operations Center (SOC) Manager |
| Status | Approved |

---

**End of Procedure**