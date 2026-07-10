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

---

# 11. Social Engineering Testing

Where approved by executive management and Legal, the organization may conduct controlled social engineering assessments to evaluate personnel awareness and organizational resilience.

Social engineering testing may include:

- Phishing simulations.
- Spear phishing assessments.
- Business Email Compromise (BEC) simulations.
- Vishing (voice phishing) assessments.
- Smishing (SMS phishing) assessments.
- Physical access testing.
- Tailgating assessments.
- Impersonation scenarios.
- Security awareness validation.
- Reporting of identified weaknesses.

Social engineering assessments shall:

- Be approved before execution.
- Avoid unnecessary disruption to business operations.
- Protect employee privacy.
- Comply with applicable legal and regulatory requirements.

---

# 12. Remediation Verification and Retesting

All identified penetration testing findings shall undergo remediation verification and retesting.

Requirements include:

- Assignment of remediation ownership.
- Risk-based prioritization.
- Validation of corrective actions.
- Retesting of remediated findings.
- Verification of compensating controls where applicable.
- Documentation of remediation evidence.
- Closure of findings only after successful validation.
- Escalation of overdue remediation activities.
- Tracking of recurring findings.
- Maintenance of remediation history.

Critical and High-risk findings shall be retested before closure.

---

# 13. Penetration Testing Reporting

A formal penetration testing report shall be produced for every authorized engagement.

Reports shall include:

- Executive summary.
- Scope of testing.
- Rules of Engagement.
- Testing methodology.
- Systems tested.
- Findings summary.
- Risk ratings.
- Technical evidence.
- Proof-of-concept details where appropriate.
- Screenshots supporting findings.
- Business impact assessment.
- Recommended remediation actions.
- Retest results where applicable.
- Overall security posture assessment.

Reports shall be classified according to the organization's Information Classification Standard.

---

# 14. Metrics and Key Performance Indicators (KPIs)

The organization shall establish metrics to evaluate the effectiveness of penetration testing activities.

Metrics shall include:

- Number of penetration tests completed.
- Percentage of critical assets tested.
- Number of Critical findings.
- Number of High findings.
- Average remediation time.
- Percentage of overdue remediation activities.
- Percentage of findings successfully retested.
- Recurring vulnerability trends.
- Third-party penetration testing coverage.
- Executive penetration testing dashboard.

Metrics shall be reviewed regularly by executive management and the Information Security Governance Committee.

---

# 15. Third-Party Penetration Testing

Third-party service providers responsible for hosting, processing, or managing organizational information shall support penetration testing activities where contractually permitted.

Requirements include:

- Review of third-party penetration testing reports.
- Verification of remediation of identified findings.
- Validation of independent security assessments.
- Review of regulatory compliance evidence.
- Coordination of testing schedules.
- Contractual penetration testing clauses.
- Protection of shared environments.
- Approval of testing activities affecting third-party services.
- Documentation of third-party testing outcomes.
- Integration with the Enterprise Third-Party Risk Management Program.

Third-party penetration testing shall be coordinated with vendor management and legal representatives.

---

# 16. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve enterprise penetration testing requirements.
- Review significant penetration testing results.
- Ensure compliance with applicable regulations and security frameworks.

## Information Security Team

The Information Security Team shall:

- Develop and maintain penetration testing procedures.
- Coordinate penetration testing engagements.
- Validate testing methodologies.
- Review penetration testing reports.
- Track remediation activities.
- Report penetration testing metrics.

## Penetration Testing Team

The Penetration Testing Team shall:

- Conduct authorized penetration tests.
- Follow approved Rules of Engagement.
- Protect organizational information during testing.
- Document technical findings.
- Produce formal penetration testing reports.
- Support remediation verification activities.

## Information Technology Team

The Information Technology Team shall:

- Support authorized testing activities.
- Coordinate maintenance windows where required.
- Remediate identified vulnerabilities.
- Validate corrective actions.
- Support retesting activities.

## System Owners

System Owners shall:

- Approve testing of assigned systems.
- Ensure systems are available during approved testing windows.
- Review penetration testing findings.
- Coordinate remediation activities.
- Request approved exceptions where justified.

## Internal Audit

Internal Audit shall:

- Review compliance with this standard.
- Validate remediation of audit findings.
- Assess penetration testing governance.
- Report material deficiencies to executive management.

## Users

Users shall:

- Cooperate with authorized penetration testing activities.
- Report suspected security issues.
- Comply with organizational security requirements.
- Refrain from interfering with approved testing activities.