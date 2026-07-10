# STD-006 Enterprise Windows Server Hardening Standard

**Document ID:** STD-006

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

The purpose of this Enterprise Windows Server Hardening Standard is to establish mandatory security configuration requirements for Microsoft Windows Server systems deployed across the enterprise.

This standard defines the minimum hardening controls necessary to reduce attack surfaces, strengthen system security, protect enterprise workloads, and support regulatory compliance through standardized Windows Server security baselines.

---

# 2. Scope

This standard applies to:

- Windows Server operating systems.
- Domain Controllers.
- Member Servers.
- File Servers.
- Print Servers.
- Application Servers.
- Database Servers.
- Virtual Windows Servers.
- Cloud-hosted Windows Servers.
- Disaster Recovery Windows Servers.
- Development and testing Windows Server environments.

This standard applies to all Windows Server systems owned, operated, or managed by the organization.

---

# 3. Objectives

The objectives of this standard are to:

- Establish secure Windows Server baselines.
- Reduce operating system attack surfaces.
- Standardize Windows Server security configurations.
- Protect enterprise services.
- Support Zero Trust Architecture.
- Improve regulatory compliance.
- Strengthen identity security.
- Improve audit readiness.
- Reduce configuration drift.
- Improve enterprise cyber resilience.

---

# 4. Standard Statement

All Windows Server systems shall be deployed, configured, maintained, and monitored using approved enterprise hardening baselines.

Windows Server configurations shall align with:

- CIS Microsoft Windows Server Benchmarks
- Microsoft Security Baselines
- NIST SP 800-53 Rev. 5
- NIST SP 800-123
- ISO/IEC 27001:2022
- Organizational security requirements

Unsupported operating systems shall not be deployed within the enterprise production environment unless formally approved through the Enterprise Exception Management process.

---

# 5. Windows Server Installation Requirements

Windows Server installations shall follow approved enterprise build standards and secure deployment procedures.

Installation requirements include:

- Use only organization-approved Windows Server versions.
- Deploy standardized enterprise server images.
- Remove unnecessary roles and features before production deployment.
- Assign unique hostnames following enterprise naming conventions.
- Join servers to the enterprise Active Directory domain where applicable.
- Configure secure time synchronization.
- Enable Secure Boot where supported.
- Validate system integrity before production deployment.

Only authorized Information Technology personnel may deploy Windows Server systems.

---

# 6. Operating System Hardening

All Windows Server systems shall be hardened prior to deployment into production.

Hardening requirements include:

- Disable unnecessary services.
- Disable unused ports and protocols.
- Remove or disable unnecessary software.
- Configure secure file system permissions.
- Disable legacy authentication protocols where possible.
- Enable User Account Control (UAC).
- Restrict anonymous access.
- Configure secure network settings.
- Enable exploit protection features.
- Apply approved security baselines.

Operating system hardening shall align with CIS Benchmarks and Microsoft Security Baselines.

---

# 7. Local Security Policies

Windows Local Security Policies shall be configured using approved enterprise security settings.

Minimum requirements include:

- Account lockout policies.
- Password complexity enforcement.
- Minimum password length.
- Audit policy configuration.
- User rights assignment.
- Security options configuration.
- Interactive logon restrictions.
- Administrative privilege restrictions.

Local policy settings shall not conflict with enterprise Group Policy Objects (GPOs).

---

# 8. Group Policy Security Settings

Enterprise Windows Servers shall receive centrally managed Group Policy Objects (GPOs).

Group Policy requirements include:

- Password policies.
- Account lockout policies.
- Windows Defender settings.
- Firewall configuration.
- Security auditing.
- PowerShell logging.
- BitLocker settings where applicable.
- Windows Update configuration.
- Remote Desktop restrictions.
- Administrative template security settings.

Unauthorized modification of enterprise GPOs is prohibited.

---

# 9. Account Security

Administrative and local accounts shall be secured using enterprise identity management controls.

Requirements include:

- Disable or rename default local administrator accounts where appropriate.
- Enforce Multi-Factor Authentication (MFA) for privileged administrative access where supported.
- Remove unused local accounts.
- Restrict local administrator group membership.
- Enforce least privilege.
- Use unique administrative accounts.
- Monitor privileged account activity.
- Disable guest accounts.

Administrative accounts shall comply with the Enterprise Identity and Access Management (IAM) Standard and Enterprise Privileged Access Management (PAM) Standard.

---

# 10. Windows Defender and Endpoint Protection

Enterprise Windows Servers shall be protected using approved endpoint security technologies.

Requirements include:

- Microsoft Defender Antivirus or an approved enterprise endpoint protection solution.
- Microsoft Defender for Endpoint (or equivalent EDR solution) where deployed.
- Real-time protection enabled.
- Automatic signature updates.
- Scheduled malware scans.
- Tamper protection enabled where supported.
- Cloud-delivered protection enabled where approved.
- Detection and response monitoring integrated with the Security Operations Center (SOC).

Endpoint protection configurations shall be monitored continuously.

---

# 11. Windows Firewall Configuration

Windows Defender Firewall shall be enabled on all Windows Server systems unless an approved exception exists.

Firewall requirements include:

- Enable firewall profiles for Domain, Private, and Public networks as appropriate.
- Block inbound traffic by default unless explicitly authorized.
- Allow only approved services and ports.
- Log firewall events.
- Review firewall rules periodically.
- Remove obsolete firewall rules.
- Restrict administrative management interfaces.
- Document firewall exceptions.

Firewall configurations shall align with enterprise network security requirements.

---

# 12. Remote Desktop (RDP) Hardening

Remote Desktop Protocol (RDP) shall be secured before being enabled on any Windows Server.

RDP security requirements include:

- Enable RDP only when required.
- Restrict RDP access to authorized administrators.
- Require Multi-Factor Authentication (MFA) where supported.
- Require Network Level Authentication (NLA).
- Restrict RDP through firewalls and network segmentation.
- Log all RDP sessions.
- Monitor failed RDP authentication attempts.
- Disable RDP when no longer required.

Direct exposure of RDP services to the public Internet is prohibited unless explicitly approved and protected by compensating security controls.

---

# 13. Patch Management

Windows Server systems shall be maintained with current security updates to reduce exposure to known vulnerabilities.

Patch management requirements include:

- Deploy Microsoft security updates in accordance with the Enterprise Patch Management Policy.
- Apply critical security patches within organization-defined service level objectives (SLOs).
- Test patches in non-production environments prior to production deployment where appropriate.
- Verify successful installation of security updates.
- Document approved maintenance windows.
- Monitor patch deployment status.
- Remediate failed patch installations promptly.
- Maintain patch compliance records.

Emergency security patches shall follow the organization's emergency change management procedures.

---

# 14. BitLocker and Disk Encryption

Enterprise Windows Servers shall use approved encryption technologies to protect sensitive information stored on local disks.

Encryption requirements include:

- Enable BitLocker where supported.
- Use Trusted Platform Module (TPM) protection where available.
- Store recovery keys securely.
- Protect encryption keys using approved enterprise key management solutions.
- Encrypt operating system volumes.
- Encrypt data volumes containing sensitive information.
- Monitor encryption status.
- Periodically validate recovery procedures.

Encryption exceptions shall be documented and approved.

---

# 15. PowerShell Security

PowerShell shall be configured securely to reduce the risk of unauthorized script execution and administrative misuse.

Requirements include:

- Enable PowerShell logging.
- Enable Script Block Logging.
- Enable Module Logging.
- Enable PowerShell Transcription where appropriate.
- Restrict execution policies based on organizational requirements.
- Digitally sign administrative scripts where feasible.
- Restrict PowerShell access to authorized administrators.
- Monitor PowerShell activity using centralized logging.

PowerShell activity shall be reviewed as part of the organization's security monitoring program.

---

# 16. Event Logging and Auditing

Windows Server systems shall generate security logs sufficient to support monitoring, investigations, and compliance.

Logging requirements include:

- Successful logon events.
- Failed logon events.
- Account management events.
- Privilege use events.
- Process creation events.
- PowerShell activity.
- Object access events where required.
- Policy change events.
- System startup and shutdown events.
- Windows Defender events.

Windows Event Logs shall be forwarded to the organization's centralized Security Information and Event Management (SIEM) platform where applicable.

---

# 17. Backup and Recovery Configuration

Windows Server systems shall be configured to support secure backup and recovery operations.

Requirements include:

- Scheduled backups of critical systems.
- Encryption of backup data.
- Secure storage of backup media.
- Protection against unauthorized backup modification.
- Periodic restoration testing.
- Backup integrity validation.
- Retention in accordance with organizational policy.
- Monitoring of backup success and failures.

Backup configurations shall align with the Enterprise Backup and Recovery Policy.

---

# 18. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve Windows Server security baseline requirements.
- Review server hardening risks.
- Ensure compliance with applicable regulations and security frameworks.

## Information Security Team

The Information Security Team shall:

- Develop and maintain Windows Server hardening baselines.
- Monitor compliance with security configuration requirements.
- Conduct periodic security assessments.
- Review security exceptions.
- Recommend improvements to server security controls.

## Information Technology Team

The Information Technology Team shall:

- Deploy Windows Servers using approved secure baseline configurations.
- Apply security updates and configuration changes.
- Configure logging, monitoring, and endpoint protection.
- Perform routine compliance checks.
- Remediate identified configuration deficiencies.

## System Owners

System Owners shall:

- Ensure Windows Servers remain compliant with this standard.
- Support vulnerability remediation.
- Approve business-related configuration changes.
- Participate in periodic compliance reviews.

## Administrators

Windows Server Administrators shall:

- Follow approved hardening procedures.
- Use privileged accounts only for administrative activities.
- Protect administrative credentials.
- Report security incidents promptly.
- Comply with enterprise change management requirements.