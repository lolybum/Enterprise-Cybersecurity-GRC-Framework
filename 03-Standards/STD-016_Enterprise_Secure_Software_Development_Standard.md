# STD-016 Enterprise Secure Software Development (Secure SDLC) Standard

**Document ID:** STD-016

**Version:** 1.0

**Owner:** Chief Information Security Officer (CISO)

**Approved By:** Executive Management

**Effective Date:** July 2026

**Review Cycle:** Annual

**Classification:** Internal

**Supporting Policies:**

- GOV-024 Enterprise Security Architecture Policy
- GOV-027 Enterprise Data Protection Policy
- GOV-029 Enterprise Vulnerability Management Policy
- GOV-040 Enterprise Incident Management Policy
- GOV-049 Enterprise Zero Trust Architecture Policy

---

# 1. Purpose

The purpose of this Enterprise Secure Software Development (Secure SDLC) Standard is to establish mandatory security requirements that integrate cybersecurity practices into every phase of the Software Development Life Cycle (SDLC).

This standard ensures that enterprise software is designed, developed, tested, deployed, and maintained using secure development practices that reduce vulnerabilities, protect organizational information, and support regulatory compliance.

---

# 2. Scope

This standard applies to:

- Internally developed applications.
- Commercial off-the-shelf (COTS) applications requiring customization.
- Web applications.
- Mobile applications.
- APIs and microservices.
- Cloud-native applications.
- Containers and Kubernetes workloads.
- DevSecOps pipelines.
- Infrastructure-as-Code (IaC).
- Software developed by third-party vendors on behalf of the organization.

This standard applies to all software development activities performed for or on behalf of the organization.

---

# 3. Objectives

The objectives of this standard are to:

- Integrate security into the SDLC.
- Reduce software vulnerabilities.
- Standardize secure coding practices.
- Improve application security.
- Support DevSecOps.
- Protect organizational information.
- Improve software resilience.
- Support regulatory compliance.
- Reduce application security risk.
- Promote secure software delivery.

---

# 4. Standard Statement

The organization shall integrate security controls into every phase of the Software Development Life Cycle (SDLC), including planning, design, development, testing, deployment, maintenance, and retirement.

All software shall be developed using approved secure development practices, validated through security testing, and deployed only after meeting enterprise security requirements.

Secure SDLC activities shall be documented, monitored, and continuously improved through governance, risk management, and quality assurance processes.

---

# 5. Secure SDLC Governance

The organization shall establish governance processes to ensure security is integrated into every phase of the Software Development Life Cycle (SDLC).

Secure SDLC governance requirements include:

- Documented Secure SDLC methodology.
- Defined security roles and responsibilities.
- Secure development policies and standards.
- Security checkpoints throughout the SDLC.
- Risk-based application security reviews.
- Secure development training for developers.
- Third-party software development oversight.
- Periodic Secure SDLC maturity assessments.

Secure SDLC governance shall be reviewed at least annually or following significant technology, regulatory, or business changes.

---

# 6. Secure Design and Threat Modeling

Security requirements shall be incorporated during the application design phase.

Requirements include:

- Security architecture review.
- Data flow analysis.
- Threat modeling for new applications and major enhancements.
- Identification of trust boundaries.
- Secure authentication design.
- Secure authorization design.
- Secure session management.
- Input validation design.
- Secure error handling.
- Privacy-by-design principles where applicable.

Threat models shall be updated whenever significant architectural changes occur.

---

# 7. Secure Coding Requirements

Software shall be developed using secure coding practices that minimize security vulnerabilities.

Secure coding requirements include:

- Compliance with approved secure coding standards.
- Validation of all user input.
- Output encoding to prevent injection attacks.
- Parameterized queries for database access.
- Secure authentication implementation.
- Secure authorization enforcement.
- Secure session management.
- Proper error handling without exposing sensitive information.
- Protection of sensitive data.
- Secure cryptographic implementation.
- Avoidance of hard-coded credentials or secrets.

Developers shall follow the organization's approved secure coding guidelines.

---

# 8. Source Code Management

Enterprise source code shall be managed using approved version control systems.

Requirements include:

- Centralized source code repositories.
- Role-Based Access Control (RBAC).
- Multi-Factor Authentication (MFA) for repository access.
- Branch protection rules.
- Mandatory pull requests for protected branches.
- Version history preservation.
- Audit logging of repository activities.
- Secure backup of source code repositories.
- Protection of sensitive branches.
- Controlled release tagging.

Access to source code repositories shall follow the Principle of Least Privilege.

---

# 9. Code Review Requirements

Security-focused code reviews shall be performed before production deployment.

Code review requirements include:

- Independent peer review.
- Verification of secure coding practices.
- Review of authentication logic.
- Review of authorization controls.
- Validation of cryptographic implementations.
- Review of logging and error handling.
- Review of third-party library usage.
- Documentation of review findings.
- Resolution of identified security issues prior to release.
- Approval by designated reviewers.

High-risk applications may require additional security review by the Information Security Team.

---

# 10. Static Application Security Testing (SAST)

Static Application Security Testing (SAST) shall be integrated into the Secure SDLC.

SAST requirements include:

- Automated source code scanning.
- Scanning of every major release.
- Scanning of high-risk code changes.
- Detection of common coding vulnerabilities.
- Integration into Continuous Integration/Continuous Deployment (CI/CD) pipelines.
- Risk-based prioritization of findings.
- Tracking of remediation activities.
- Verification of vulnerability resolution.
- Documentation of scan results.
- Continuous improvement of scanning rules.

Critical and High-risk SAST findings shall be remediated or formally accepted through the Enterprise Risk Acceptance process before production deployment.

---

# 11. Dynamic Application Security Testing (DAST)

Dynamic Application Security Testing (DAST) shall be performed against running applications to identify security vulnerabilities that may not be detected through static analysis.

DAST requirements include:

- Automated dynamic security scanning.
- Testing in staging or pre-production environments.
- Authentication-enabled scanning where appropriate.
- Detection of OWASP Top 10 vulnerabilities.
- Validation of authentication controls.
- Validation of authorization controls.
- Detection of security misconfigurations.
- Testing of exposed APIs.
- Documentation of scan results.
- Verification of remediation activities.

Critical and High-risk DAST findings shall be remediated or formally accepted before production deployment.

---

# 12. Software Composition Analysis (SCA)

Software Composition Analysis (SCA) shall be used to identify security risks associated with third-party and open-source software components.

SCA requirements include:

- Inventory of third-party software components.
- Identification of vulnerable dependencies.
- Continuous monitoring of software components.
- License compliance verification.
- Detection of outdated libraries.
- Risk-based prioritization of vulnerable components.
- Verification of dependency updates.
- Documentation of remediation activities.
- Integration into CI/CD pipelines.
- Continuous monitoring of software supply chain risks.

Unsupported or high-risk software components shall not be deployed into production without documented risk acceptance.

---

# 13. CI/CD Pipeline Security

Continuous Integration and Continuous Deployment (CI/CD) pipelines shall implement security controls that protect software throughout the build and deployment process.

CI/CD security requirements include:

- Secure build environments.
- Multi-Factor Authentication (MFA) for pipeline administrators.
- Role-Based Access Control (RBAC).
- Protection of build artifacts.
- Secure storage of secrets and credentials.
- Automated security testing.
- Artifact integrity verification.
- Audit logging of pipeline activities.
- Separation of development, testing, and production environments.
- Periodic review of pipeline configurations.

CI/CD pipelines shall be protected from unauthorized modification.

---

# 14. DevSecOps Requirements

Security shall be integrated into DevOps processes through a DevSecOps approach.

DevSecOps requirements include:

- Automated security testing.
- Infrastructure-as-Code (IaC) security scanning.
- Container image scanning.
- Secrets detection.
- Continuous compliance monitoring.
- Security gates within deployment pipelines.
- Automated policy enforcement.
- Continuous vulnerability management.
- Integration with enterprise SIEM where appropriate.
- Continuous improvement of DevSecOps practices.

Security controls shall be implemented as early as possible in the software development lifecycle.

---

# 15. Release Management

Software releases shall follow an approved release management process prior to production deployment.

Release management requirements include:

- Documented release approvals.
- Successful completion of required security testing.
- Resolution of Critical and High-risk vulnerabilities or approved risk acceptance.
- Verification of change management approvals.
- Deployment rollback procedures.
- Release documentation.
- Production deployment monitoring.
- Post-release validation.
- Secure storage of release artifacts.
- Version control of released software.

Emergency releases shall follow the organization's Emergency Change Management process.

---

# 16. Roles and Responsibilities

## Chief Information Security Officer (CISO)

The CISO shall:

- Own this standard.
- Approve Secure SDLC requirements.
- Review application security risks.
- Ensure compliance with applicable regulations and security frameworks.

## Application Security Team

The Application Security Team shall:

- Develop Secure SDLC requirements.
- Conduct application security assessments.
- Review threat models.
- Maintain SAST, DAST, and SCA tooling.
- Produce application security metrics.
- Recommend improvements to Secure SDLC practices.

## Development Team

The Development Team shall:

- Follow approved secure coding standards.
- Remediate identified security vulnerabilities.
- Participate in code reviews.
- Support security testing.
- Maintain secure source code repositories.
- Participate in Secure SDLC training.

## DevOps / Platform Engineering Team

The DevOps / Platform Engineering Team shall:

- Secure CI/CD pipelines.
- Maintain build infrastructure.
- Protect deployment credentials.
- Support automated security testing.
- Monitor pipeline security events.
- Implement Infrastructure-as-Code (IaC) security controls.

## System Owners

System Owners shall:

- Ensure applications comply with this standard.
- Participate in application risk assessments.
- Approve production releases.
- Review security findings.
- Request approved exceptions where necessary.

## Users

Users shall:

- Report suspected application security issues.
- Protect application credentials.
- Use enterprise applications in accordance with organizational policies.
- Cooperate with authorized security investigations.