# STD-024 Enterprise Penetration Testing Standard

**Document ID:** STD-024

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-024 Enterprise Security Architecture Policy
- GOV-029 Enterprise Vulnerability Management Policy
- GOV-039 Enterprise Logging and Monitoring Policy
- GOV-040 Enterprise Incident Management Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Penetration Testing Standard is to establish mandatory requirements for planning, conducting, documenting, and reporting penetration testing activities to identify exploitable security weaknesses in enterprise technology assets.

This standard defines the minimum requirements for internal and external penetration testing, web application testing, API testing, cloud security testing, wireless security testing, and remediation verification to strengthen the organization's cybersecurity posture.

---

# 2. Scope

This standard applies to:

- Internal networks.
- External networks.
- Windows servers.
- Linux servers.
- Cloud infrastructure.
- Web applications.
- APIs.
- Mobile applications where applicable.
- Wireless networks.
- Containers and Kubernetes clusters.
- Identity and Access Management (IAM) services.
- Critical enterprise applications.
- Third-party hosted systems where contractually permitted.

This standard applies to all enterprise-managed systems that process, store, or transmit organizational information.

---

# 3. Objectives

The objectives of this standard are to:

- Identify exploitable security weaknesses.
- Validate security controls.
- Reduce organizational cyber risk.
- Improve vulnerability remediation.
- Support regulatory compliance.
- Strengthen secure system design.
- Improve incident preparedness.
- Validate defensive security capabilities.
- Enhance cyber resilience.
- Support continuous security improvement.

---

# 4. Standard Statement

The organization shall perform risk-based penetration testing using qualified personnel, approved methodologies, and authorized testing tools.

Penetration testing shall simulate realistic attack scenarios while minimizing operational disruption and protecting the confidentiality, integrity, and availability of enterprise systems.

Testing activities shall be documented, approved, monitored, and integrated with enterprise vulnerability management and risk management processes.

---

# 5. Penetration Testing Governance

The organization shall establish governance processes to ensure penetration testing activities are properly authorized, planned, executed, documented, and reviewed.

Penetration testing governance requirements include:

- Documented penetration testing procedures.
- Defined governance roles and responsibilities.
- Executive approval for penetration testing activities.
- Integration with Enterprise Risk Management (ERM).
- Coordination with Change Management processes.
- Coordination with Incident Response teams.
- Protection of production systems during testing.
- Continuous improvement of penetration testing capabilities.

Penetration testing governance shall be reviewed at least annually or following significant business, regulatory, technology, or threat landscape changes.

---

# 6. Rules of Engagement

All penetration testing activities shall be governed by documented Rules of Engagement (RoE) approved before testing begins.

Rules of Engagement shall define:

- Testing objectives.
- Scope of testing.
- In-scope assets.
- Out-of-scope assets.
- Approved testing windows.
- Authorized testing techniques.
- Communication procedures.
- Emergency contact information.
- Incident escalation procedures.
- Conditions requiring immediate suspension of testing.

Testing shall not begin until the Rules of Engagement have been reviewed and approved by all relevant stakeholders.

---

# 7. Internal and External Penetration Testing

The organization shall conduct both internal and external penetration testing based on business risk and regulatory requirements.

Internal penetration testing shall evaluate:

- Internal network security.
- Active Directory security.
- Identity and Access Management (IAM).
- Privileged account protections.
- Lateral movement opportunities.
- Internal application security.
- Segmentation effectiveness.
- Endpoint security controls.

External penetration testing shall evaluate:

- Internet-facing infrastructure.
- Public web applications.
- VPN gateways.
- Remote access solutions.
- Public APIs.
- External DNS infrastructure.
- Email security infrastructure.
- Cloud-hosted public services.

Testing shall simulate realistic attacker techniques while minimizing operational disruption.

---

# 8. Web Application and API Penetration Testing

Enterprise web applications and APIs shall undergo penetration testing using recognized industry methodologies.

Testing requirements include:

- OWASP Web Security Testing Guide (WSTG).
- OWASP Top 10 validation.
- OWASP API Security Top 10 validation.
- Authentication testing.
- Authorization testing.
- Session management testing.
- Input validation testing.
- Business logic testing.
- Cryptographic control validation.
- Security misconfiguration testing.

Critical business applications shall undergo penetration testing prior to production deployment and following significant architectural changes.

---

# 9. Cloud and Wireless Penetration Testing

Cloud-hosted services and enterprise wireless environments shall be assessed through authorized penetration testing activities.

Cloud penetration testing requirements include:

- Cloud infrastructure assessments.
- Cloud identity security testing.
- Cloud storage security validation.
- Cloud network security testing.
- Container security assessments.
- Kubernetes security testing.
- API gateway security testing.
- Validation of cloud security controls.

Wireless penetration testing requirements include:

- Wireless authentication testing.
- Wireless encryption validation.
- Rogue access point detection.
- Guest wireless security testing.
- Wireless segmentation validation.

Testing shall comply with cloud provider policies and contractual requirements.

---

# 10. Testing Frequency

Penetration testing shall be performed according to organizational risk, asset criticality, and regulatory requirements.

Minimum testing frequencies include:

- Internet-facing critical systems: At least annually.
- Critical business applications: Prior to production deployment and annually thereafter.
- Public APIs: Prior to production deployment and annually thereafter.
- Cloud environments: Annually and following significant architectural changes.
- Wireless infrastructure: Annually.
- Internal networks: At least annually.
- Following major infrastructure changes.
- Following significant security incidents.
- As required by regulatory or contractual obligations.

Additional penetration testing may be conducted based on emerging threats, business requirements, or executive management direction.