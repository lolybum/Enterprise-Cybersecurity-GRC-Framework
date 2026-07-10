# STD-008 Enterprise Endpoint Protection Standard

**Document ID:** STD-008

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-025 Enterprise Endpoint Security Policy
- GOV-029 Enterprise Vulnerability Management Policy
- GOV-030 Enterprise Patch Management Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-040 Enterprise Incident Management Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Endpoint Protection Standard is to establish mandatory security requirements for protecting enterprise endpoints against malware, ransomware, unauthorized access, malicious software, and other cyber threats.

This standard defines the minimum security controls required to secure desktops, laptops, mobile devices, virtual endpoints, and other endpoint systems while supporting the organization's Zero Trust Architecture and cybersecurity resilience objectives.

---

# 2. Scope

This standard applies to:

- Desktop computers.
- Laptop computers.
- Windows endpoints.
- Linux endpoints.
- macOS endpoints.
- Virtual desktops.
- Corporate mobile devices.
- Bring Your Own Device (BYOD) systems approved for enterprise access.
- Endpoint Detection and Response (EDR) platforms.
- Antivirus and anti-malware solutions.
- Remote endpoints.
- Cloud-managed endpoints.

This standard applies to all enterprise-managed endpoint devices that connect to organizational networks or process organizational information.

---

# 3. Objectives

The objectives of this standard are to:

- Protect enterprise endpoints from cyber threats.
- Reduce malware and ransomware risks.
- Standardize endpoint security controls.
- Strengthen endpoint visibility.
- Improve threat detection and response.
- Support Zero Trust Architecture.
- Enhance regulatory compliance.
- Protect organizational information assets.
- Improve incident response capabilities.
- Strengthen enterprise cyber resilience.

---

# 4. Standard Statement

The organization shall implement enterprise endpoint protection controls that prevent, detect, respond to, and recover from endpoint security threats.

All enterprise endpoints shall be protected using approved endpoint security technologies, continuously monitored for suspicious activity, and maintained in accordance with approved enterprise security baselines.

Endpoint protection controls shall integrate with centralized security monitoring and incident response processes.

---

# 5. Endpoint Detection and Response (EDR)

The organization shall deploy an approved Endpoint Detection and Response (EDR) solution on all supported enterprise endpoints.

EDR requirements include:

- Continuous endpoint monitoring.
- Behavioral threat detection.
- Real-time threat intelligence integration.
- Automated threat containment where appropriate.
- Endpoint isolation capabilities.
- Detection of ransomware activity.
- Detection of malicious scripts.
- Detection of privilege escalation attempts.
- Centralized alerting.
- Integration with the Security Information and Event Management (SIEM) platform.

EDR agents shall remain active and shall not be disabled without documented approval.

---

# 6. Antivirus and Anti-Malware Protection

All enterprise endpoints shall use an approved antivirus and anti-malware solution.

Requirements include:

- Real-time malware protection.
- Automatic signature updates.
- Scheduled full-system scans.
- On-access file scanning.
- Detection of ransomware.
- Detection of spyware.
- Detection of potentially unwanted applications (PUAs).
- Cloud-assisted threat intelligence where approved.
- Tamper protection enabled.
- Automatic quarantine of detected threats.

Users shall not disable antivirus protection without authorization.

---

# 7. Endpoint Configuration Requirements

Enterprise endpoints shall be configured using approved secure baseline configurations.

Configuration requirements include:

- Approved operating system images.
- Secure boot enabled where supported.
- Automatic operating system updates.
- Approved endpoint security software.
- Disk encryption enabled.
- Screen lock after inactivity.
- Removal of unnecessary software.
- Restriction of local administrator privileges.
- Secure browser configuration.
- Continuous compliance monitoring.

Endpoint configurations shall align with the Enterprise Secure Configuration Baseline Standard.

---

# 8. Host Firewall Requirements

A host-based firewall shall be enabled on all enterprise endpoints.

Firewall requirements include:

- Enable firewall by default.
- Block unsolicited inbound connections.
- Permit only approved services and applications.
- Log firewall events.
- Prevent unauthorized firewall rule changes.
- Apply enterprise-managed firewall policies.
- Periodically review firewall configurations.
- Document approved firewall exceptions.

Firewall settings shall be centrally managed wherever technically feasible.

---

# 9. Device Control (USB and Removable Media)

Use of removable media shall be controlled to reduce the risk of malware infections and unauthorized data transfer.

Requirements include:

- Restrict unauthorized USB storage devices.
- Approve removable media through documented business processes.
- Automatically scan removable media for malware.
- Encrypt approved removable storage devices.
- Log removable media usage.
- Block unauthorized peripheral devices where appropriate.
- Disable AutoRun and AutoPlay features.
- Monitor removable media activity.

Exceptions shall require documented approval.

---

# 10. Application Control and Allowlisting

Application execution shall be controlled using approved application control technologies.

Requirements include:

- Maintain an approved software inventory.
- Permit execution of authorized applications only where feasible.
- Block unauthorized software.
- Prevent execution of known malicious applications.
- Restrict script execution based on enterprise policy.
- Review application allowlists periodically.
- Validate software before deployment.
- Monitor application execution events.

Application control policies shall support business operations while reducing endpoint security risk.

---

# 11. Endpoint Encryption

Enterprise endpoints shall use approved encryption technologies to protect organizational information from unauthorized access.

Encryption requirements include:

- Full disk encryption shall be enabled on all enterprise-managed laptops.
- Full disk encryption shall be enabled on desktops where required by risk assessment or regulatory requirements.
- Approved encryption technologies shall be used (e.g., BitLocker, FileVault, LUKS, or equivalent).
- Encryption keys shall be securely managed using approved enterprise key management solutions.
- Recovery keys shall be securely stored and protected.
- Removable storage devices containing organizational data shall be encrypted.
- Encryption status shall be monitored continuously.
- Encryption failures shall be investigated and remediated promptly.

---

# 12. Mobile Endpoint Security

Enterprise-managed mobile devices shall comply with approved mobile security requirements.

Requirements include:

- Mobile Device Management (MDM) enrollment.
- Device encryption enabled.
- Screen lock using PIN, password, or biometric authentication.
- Automatic device lock after inactivity.
- Approved application installation only.
- Remote lock and remote wipe capability.
- Operating system updates enabled.
- Detection of jailbroken or rooted devices.
- Separation of corporate and personal data where applicable.
- Continuous compliance monitoring.

Non-compliant mobile devices shall not be permitted to access enterprise resources.

---

# 13. Endpoint Monitoring

Enterprise endpoints shall be continuously monitored to detect security threats and operational issues.

Monitoring activities include:

- Endpoint health status.
- Malware detection events.
- EDR alerts.
- Firewall events.
- Authentication events.
- Privilege escalation attempts.
- Configuration changes.
- Software installation events.
- USB device usage.
- Encryption status.

Endpoint monitoring shall integrate with centralized security monitoring platforms.

---

# 14. Vulnerability Management Integration

Enterprise endpoint protection shall integrate with the organization's Vulnerability Management Program.

Requirements include:

- Scheduled vulnerability scanning.
- Identification of missing security patches.
- Detection of unsupported software.
- Risk-based vulnerability prioritization.
- Verification of remediation activities.
- Reporting of vulnerability trends.
- Integration with asset inventory systems.
- Continuous monitoring of endpoint risk posture.

Critical vulnerabilities shall be remediated in accordance with the Enterprise Vulnerability Management Policy.

---

# 15. Incident Response Integration

Endpoint protection technologies shall support the Enterprise Incident Response Program.

Requirements include:

- Automated alert generation.
- Endpoint isolation capabilities.
- Collection of forensic artifacts.
- Threat intelligence integration.
- Malware containment.
- Incident ticket generation.
- Secure evidence preservation.
- Support for post-incident analysis.

Endpoint security events shall be escalated to the Security Operations Center (SOC) in accordance with the Enterprise Incident Management Policy.

---

# 16. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve enterprise endpoint protection requirements.
- Review endpoint security risks.
- Ensure alignment with applicable regulations and security frameworks.

## Information Security Team

The Information Security Team shall:

- Develop and maintain endpoint protection standards.
- Monitor endpoint security events.
- Review malware and ransomware incidents.
- Conduct endpoint security assessments.
- Recommend improvements to endpoint security controls.

## Information Technology Team

The Information Technology Team shall:

- Deploy and maintain endpoint protection solutions.
- Configure EDR, antivirus, firewall, and encryption technologies.
- Perform endpoint security updates.
- Monitor endpoint compliance.
- Remediate identified endpoint security issues.

## Managers

Managers shall:

- Ensure personnel comply with endpoint security requirements.
- Support endpoint security awareness.
- Report endpoint-related security concerns.

## Users

Users shall:

- Use only approved enterprise endpoint devices.
- Protect assigned devices from unauthorized access.
- Promptly report lost, stolen, or compromised devices.
- Refrain from disabling security controls.
- Comply with all endpoint security requirements.
