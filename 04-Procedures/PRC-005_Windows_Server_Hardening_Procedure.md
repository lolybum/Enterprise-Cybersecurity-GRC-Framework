# PRC-005 Windows Server Hardening Procedure

**Procedure ID:** PRC-005

**Version:** 1.0

**Owner:** Infrastructure Security Manager

**Approved By:** Chief Information Security Officer (CISO)

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Documents:**

- GOV-024 Enterprise Security Architecture Policy
- STD-005 Enterprise Secure Configuration Baseline Standard
- STD-006 Enterprise Windows Server Hardening Standard
- STD-008 Enterprise Endpoint Protection Standard
- STD-009 Enterprise Network Security Standard

---

# 1. Purpose

The purpose of this procedure is to establish a standardized process for securely configuring, hardening, validating, and maintaining Microsoft Windows Server systems to reduce security risk and improve the organization's cybersecurity posture.

This procedure ensures Windows servers are configured according to approved security baselines before being placed into production and throughout their operational lifecycle.

---

# 2. Scope

This procedure applies to:

- Windows Server 2019.
- Windows Server 2022.
- Domain Controllers.
- Member Servers.
- File Servers.
- Application Servers.
- Database Servers.
- Virtual Windows Servers.
- Cloud-hosted Windows Servers.
- Disaster Recovery Windows Servers.

This procedure applies to all enterprise-managed Windows Server systems.

---

# 3. Procedure Objectives

The objectives of this procedure are to:

- Implement approved Windows security baselines.
- Reduce the attack surface.
- Strengthen authentication security.
- Protect privileged accounts.
- Improve logging and monitoring.
- Secure network communications.
- Support regulatory compliance.
- Standardize Windows server deployments.
- Support continuous security improvement.

---

# 4. Prerequisites

Before beginning server hardening activities, the following shall be completed:

- Approved server build request.
- Approved operating system version.
- Asset registration completed.
- Server ownership assigned.
- Network configuration completed.
- Required security software available.
- Latest Microsoft security updates available.
- Backup completed before implementing hardening changes.
- Change Management approval obtained.

---

# 5. Roles and Responsibilities

## Infrastructure Team

The Infrastructure Team shall:

- Build Windows Server systems.
- Install the approved operating system.
- Configure baseline settings.
- Apply approved security configurations.
- Coordinate with the Information Security Team.
- Document all hardening activities.

## Information Security Team

The Information Security Team shall:

- Maintain approved hardening baselines.
- Validate compliance with security standards.
- Perform security reviews.
- Conduct configuration assessments.
- Approve security exceptions.
- Monitor compliance.

## System Owner

The System Owner shall:

- Approve server deployment.
- Validate business requirements.
- Coordinate maintenance windows.
- Review security recommendations.
- Support remediation activities.

## Change Management

The Change Management Team shall:

- Review change requests.
- Approve production implementation.
- Maintain change records.
- Verify successful implementation.

---

# 6. Server Build Preparation

Before hardening begins, verify the server has been built according to enterprise standards.

Preparation activities include:

- Install the approved Windows Server version.
- Apply the latest supported service packs.
- Verify server hostname.
- Configure static IP addressing where required.
- Join the server to the Active Directory domain where applicable.
- Synchronize system time with approved NTP sources.
- Install approved device drivers.
- Verify system hardware health.
- Register the server within the Configuration Management Database (CMDB).

---

# 7. Operating System Hardening

The operating system shall be configured according to the approved enterprise security baseline.

Hardening requirements include:

- Remove unnecessary server roles and features.
- Remove unused software.
- Disable unnecessary services.
- Disable SMBv1.
- Enable Secure Boot where supported.
- Enable BitLocker where applicable.
- Configure Windows Update settings.
- Enable Windows Defender Tamper Protection.
- Configure User Account Control (UAC).
- Disable anonymous access where possible.
- Restrict PowerShell execution according to enterprise policy.
- Disable AutoRun and AutoPlay.
- Configure approved time synchronization.
- Apply Microsoft Security Baselines.

Operating system hardening shall be validated before production deployment.

---

# 8. Local Security Policy Configuration

Configure Local Security Policy using approved enterprise security baselines.

Configuration requirements include:

- Password policy enforcement.
- Account lockout policy.
- Kerberos policy configuration.
- Audit policy configuration.
- User Rights Assignment.
- Security Options configuration.
- Interactive logon security settings.
- Remote Desktop restrictions.
- Network security settings.
- Device control settings.
- Credential protection settings.

Only approved administrative personnel shall modify Local Security Policy.

---

# 9. Microsoft Defender Configuration

Microsoft Defender shall be configured using enterprise-approved security settings.

Configuration requirements include:

- Enable real-time protection.
- Enable cloud-delivered protection.
- Enable tamper protection.
- Enable automatic sample submission where approved.
- Enable ransomware protection where supported.
- Configure scheduled scans.
- Configure signature updates.
- Enable attack surface reduction (ASR) rules where supported.
- Integrate with Microsoft Defender for Endpoint where deployed.
- Configure alert forwarding to the SIEM platform.

Security signatures shall be updated automatically.

---

# 10. Windows Firewall Configuration

Windows Defender Firewall shall remain enabled on all network profiles.

Firewall requirements include:

- Enable Domain profile.
- Enable Private profile.
- Enable Public profile.
- Block inbound connections unless explicitly authorized.
- Restrict outbound connections where appropriate.
- Allow only approved application ports.
- Remove unused firewall rules.
- Document approved exceptions.
- Log dropped packets where appropriate.
- Forward firewall logs to the enterprise logging platform.

Firewall rules shall be reviewed periodically to ensure continued compliance with enterprise security requirements.

---

# 11. Windows Update Configuration

Windows Update shall be configured to ensure timely installation of security patches and critical updates.

Configuration requirements include:

- Enable automatic security updates where approved.
- Configure Windows Server Update Services (WSUS) or Microsoft Intune where deployed.
- Validate update source configuration.
- Install critical security updates according to the Enterprise Patch Management Standard.
- Schedule maintenance windows for updates.
- Verify successful installation of updates.
- Reboot servers when required.
- Document update failures.
- Escalate failed updates according to change management procedures.

All updates shall be validated prior to production deployment where practical.

---

# 12. Remote Desktop Security

Remote Desktop Services (RDS) shall be secured to minimize unauthorized administrative access.

Configuration requirements include:

- Enable Remote Desktop only where business justified.
- Restrict Remote Desktop access to authorized administrators.
- Require Network Level Authentication (NLA).
- Enforce Multi-Factor Authentication (MFA) where supported.
- Limit Remote Desktop access through approved firewall rules.
- Restrict access using administrative security groups.
- Disable clipboard, printer, and drive redirection where not required.
- Configure idle session timeouts.
- Enable session logging.
- Review Remote Desktop access periodically.

Remote administrative access shall be protected using enterprise-approved secure access solutions.

---

# 13. Audit Policy Configuration

Windows Audit Policies shall be configured using approved enterprise baselines.

Audit requirements include:

- Log account logon events.
- Log logon and logoff events.
- Log account management activities.
- Log privilege use.
- Log process creation events.
- Log object access where appropriate.
- Log policy changes.
- Log system events.
- Log directory service access for Domain Controllers.
- Configure advanced audit policies where supported.

Audit configurations shall support incident response, forensic investigations, and regulatory compliance.

---

# 14. Logging and Monitoring

Windows servers shall forward security logs to the enterprise logging platform.

Logging requirements include:

- Forward Windows Event Logs to the Security Information and Event Management (SIEM) platform.
- Monitor authentication events.
- Monitor privilege escalation events.
- Monitor Windows Defender alerts.
- Monitor firewall events.
- Monitor system integrity events.
- Monitor scheduled task creation.
- Monitor service creation and modification.
- Monitor PowerShell activity where appropriate.
- Configure alerts for high-risk security events.

Logs shall be protected against unauthorized modification and retained according to the Enterprise Security Logging and Monitoring Standard.

---

# 15. Validation and Compliance Checks

Following hardening activities, the server shall undergo validation to confirm compliance with enterprise requirements.

Validation activities include:

- Verify compliance with approved Windows security baselines.
- Perform vulnerability scanning.
- Review local security policy settings.
- Validate Windows Defender configuration.
- Validate Windows Firewall configuration.
- Confirm successful update installation.
- Verify audit policy configuration.
- Validate logging to the SIEM platform.
- Review privileged account configuration.
- Confirm removal of unnecessary services and software.

Servers failing validation shall not be promoted to production until corrective actions have been completed.

---

# 16. Documentation Requirements

The following records shall be maintained for each hardened Windows Server:

- Server hostname.
- Asset identifier.
- Operating system version.
- Hardening completion date.
- Security baseline version applied.
- Windows Update status.
- Firewall configuration summary.
- Audit policy configuration.
- Vulnerability scan results.
- Validation checklist.
- Exception approvals where applicable.
- Change Management records.

Documentation shall be retained in accordance with the organization's Records Retention Policy.