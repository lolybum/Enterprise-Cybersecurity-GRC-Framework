# STD-009 Enterprise Network Security Standard

**Document ID:** STD-009

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-024 Enterprise Security Architecture Policy
- GOV-026 Enterprise Network Security Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-040 Enterprise Incident Management Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Network Security Standard is to establish mandatory technical and operational requirements for securing enterprise network infrastructure, communications, and network-connected systems.

This standard defines the minimum security controls required to protect enterprise networks against unauthorized access, cyber threats, lateral movement, denial-of-service attacks, and data interception while supporting the organization's Zero Trust Architecture.

---

# 2. Scope

This standard applies to:

- Enterprise Local Area Networks (LAN).
- Wide Area Networks (WAN).
- Software-Defined Wide Area Networks (SD-WAN).
- Wireless Local Area Networks (WLAN).
- Cloud networking environments.
- Virtual Private Networks (VPN).
- Firewalls.
- Routers.
- Switches.
- Load balancers.
- Network security appliances.
- Network management platforms.
- Hybrid network environments.

This standard applies to all network infrastructure owned, managed, or operated by the organization.

---

# 3. Objectives

The objectives of this standard are to:

- Protect enterprise network infrastructure.
- Reduce network attack surfaces.
- Standardize secure network configurations.
- Prevent unauthorized network access.
- Support Zero Trust Architecture.
- Improve network visibility.
- Strengthen regulatory compliance.
- Improve network resilience.
- Detect network threats.
- Support continuous monitoring.

---

# 4. Standard Statement

The organization shall implement secure network controls that protect enterprise communications, infrastructure, and services from unauthorized access and cyber threats.

Network infrastructure shall be securely configured, continuously monitored, regularly assessed, and maintained using approved enterprise security baselines.

All network security controls shall align with enterprise risk management objectives, applicable regulatory requirements, and recognized industry security frameworks.

---

# 5. Network Segmentation

The organization shall implement network segmentation to reduce attack surfaces, limit lateral movement, and protect critical assets.

Segmentation requirements include:

- Separation of production, development, testing, and disaster recovery environments.
- Segmentation of user, server, and management networks.
- Isolation of critical business systems.
- Dedicated management networks for administrative access.
- Segmentation of Internet-facing systems.
- Restricted communication between network zones.
- Documentation of network trust boundaries.
- Periodic review of segmentation effectiveness.

Network segmentation shall align with the organization's Zero Trust Architecture.

---

# 6. Firewall Security

Enterprise firewalls shall be deployed to control network traffic entering, leaving, and traversing enterprise networks.

Firewall requirements include:

- Default deny inbound traffic unless explicitly authorized.
- Restrict outbound traffic based on business requirements.
- Implement least privilege firewall rules.
- Review firewall rules at least quarterly.
- Remove obsolete or unused rules.
- Enable firewall logging.
- Synchronize firewall system clocks with approved NTP servers.
- Restrict firewall administration to authorized personnel.

Firewall configurations shall be backed up and securely stored.

---

# 7. Router and Switch Security

Enterprise routers and switches shall be securely configured and managed.

Requirements include:

- Disable unused interfaces and ports.
- Disable insecure management protocols (e.g., Telnet).
- Use secure management protocols such as SSH and HTTPS.
- Change default administrative credentials.
- Enable centralized authentication where supported.
- Configure secure SNMP (SNMPv3).
- Maintain approved firmware versions.
- Backup network device configurations.
- Restrict administrative access.
- Enable configuration integrity monitoring.

Network device configurations shall comply with enterprise secure baseline standards.

---

# 8. Network Access Control (NAC)

Network Access Control (NAC) shall be implemented to verify endpoint compliance before granting access to enterprise networks.

NAC requirements include:

- Device authentication.
- User authentication.
- Endpoint compliance verification.
- Endpoint health assessment.
- Role-based network access.
- Guest network isolation.
- Automatic quarantine of non-compliant devices.
- Continuous endpoint compliance monitoring.

Non-compliant devices shall be denied or restricted from network access.

---

# 9. Virtual Private Network (VPN) Security

Remote access to enterprise resources shall be protected using approved VPN technologies.

VPN requirements include:

- Multi-Factor Authentication (MFA).
- Strong encryption protocols.
- Secure authentication mechanisms.
- Device compliance verification before connection.
- Continuous monitoring of VPN sessions.
- Automatic session timeout.
- Logging of VPN authentication events.
- Restriction of split tunneling unless explicitly approved.
- Risk-based authentication where supported.
- Secure termination of inactive sessions.

VPN gateways shall be regularly updated and monitored.

---

# 10. Wireless Network Security

Enterprise wireless networks shall be configured using approved security controls.

Wireless security requirements include:

- WPA3 encryption where supported.
- WPA2-Enterprise as the minimum standard where WPA3 is unavailable.
- 802.1X authentication.
- Separate guest wireless networks.
- Network segmentation for wireless clients.
- Rogue access point detection.
- Wireless intrusion detection where supported.
- Secure wireless controller management.
- Periodic wireless security assessments.
- Continuous monitoring of wireless infrastructure.

Unauthorized wireless access points are prohibited.