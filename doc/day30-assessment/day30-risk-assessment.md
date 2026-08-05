# Risk Assessment — DesertTech Solutions
**Company:** DesertTech Solutions  
**Date:** August 2026  
**Scope:** Preliminary Review Findings (Day 30 Assessment)  

---

## Risk Inventory

### Risk ID: RSK-01
* **Risk:** Unauthorized access to cloud environment via dormant accounts.
* **Asset/Data:** Microsoft 365 Environment / Corporate Data.
* **Threat:** Malicious actor or former employee compromising inactive accounts.
* **Vulnerability:** 5 former employees still have active M365 accounts (Finding A).
* **Likelihood:** Medium
* **Impact:** High
* **Inherent Risk:** High
* **Existing Control:** None (Offboarding process failed).
* **Recommended Treatment:** Immediately disable all former employee accounts and automate the offboarding checklist.
* **Residual Risk:** Low
* **Owner:** IT Manager / Helpdesk Lead

### Risk ID: RSK-02
* **Risk:** Compromise of administrative accounts leading to total tenant takeover.
* **Asset/Data:** Azure & M365 Administrative Accounts / Global Admin Privileges.
* **Threat:** Credential stuffing, phishing, or brute-force attacks targeting admins.
* **Vulnerability:** 3 privileged accounts lack Multi-Factor Authentication (Finding B).
* **Likelihood:** Medium
* **Impact:** Critical
* **Inherent Risk:** Critical
* **Existing Control:** MFA enabled for standard users.
* **Recommended Treatment:** Enforce mandatory MFA immediately for all privileged and administrative accounts via Conditional Access policies.
* **Residual Risk:** Low
* **Owner:** IT Security Lead

### Risk ID: RSK-03
* **Risk:** Data breach or non-compliance regarding outsourced employee data processing.
* **Asset/Data:** Employee Personal Data (HR records, PII).
* **Threat:** Third-party vendor security failure or unauthorized data exposure.
* **Vulnerability:** Payroll vendor has not provided current security-assessment evidence (Finding C).
* **Likelihood:** Medium
* **Impact:** High
* **Inherent Risk:** High
* **Existing Control:** Vendor contract in place (though security posture unverified).
* **Recommended Treatment:** Issue a formal request for recent SOC 2 reports or security assessments; update vendor risk management procedures.
* **Residual Risk:** Medium
* **Owner:** Procurement / HR Manager

### Risk ID: RSK-04
* **Risk:** Permanent data loss or extended operational downtime following a disruptive incident.
* **Asset/Data:** Corporate Backups / Cloud Databases.
* **Threat:** Ransomware attack, accidental deletion, or cloud storage corruption.
* **Vulnerability:** Daily backups run, but no restore tests have ever been performed (Finding D).
* **Likelihood:** Low
* **Impact:** Critical
* **Inherent Risk:** High
* **Existing Control:** Automated daily backup jobs configured.
* **Recommended Treatment:** Establish a bi-annual backup restoration testing schedule and document the recovery time objectives (RTO).
* **Residual Risk:** Low
* **Owner:** IT Infrastructure Lead

### Risk ID: RSK-05
* **Risk:** Misalignment with current business operations, evolving threats, and regulatory expectations.
* **Asset/Data:** Information Security Policy Documentation.
* **Threat:** Outdated security practices leading to compliance violations or unaddressed attack vectors.
* **Vulnerability:** Information Security Policy has not been reviewed for two years (Finding E).
* **Likelihood:** Medium
* **Impact:** Medium
* **Inherent Risk:** Medium
* **Existing Control:** Legacy security policy exists.
* **Recommended Treatment:** Conduct an immediate annual review and update of the Information Security Policy framework.
* **Residual Risk:** Low
* **Owner:** GRC Analyst / Chief Information Security Officer (CISO)

### Risk ID: RSK-06
* **Risk:** Exploitation of known vulnerabilities leading to system compromise.
* **Asset/Data:** Servers, Laptops, and Cloud Infrastructure.
* **Threat:** External hackers or malware exploiting unpatched software flaws.
* **Vulnerability:** Critical vulnerabilities left unresolved for >90 days (Finding F).
* **Likelihood:** High
* **Impact:** High
* **Inherent Risk:** Critical
* **Existing Control:** Vulnerability scanning tools are actively running.
* **Recommended Treatment:** Enforce a strict SLA for vulnerability patching (e.g., Critical flaws patched within 7–14 days).
* **Residual Risk:** Medium
* **Owner:** IT Security / Systems Administration

### Risk ID: RSK-07
* **Risk:** Regulatory penalties and reputational damage due to unregulated processing of customer personal data.
* **Asset/Data:** Customer Personal Data (UAE PDPL scope).
* **Threat:** Regulatory audit, privacy breach, or unauthorized data usage by SaaS platforms.
* **Vulnerability:** Customer personal data stored in SaaS without documented processing activities or privacy-risk assessments (Finding G).
* **Likelihood:** High
* **Impact:** High
* **Inherent Risk:** Critical
* **Existing Control:** None.
* **Recommended Treatment:** Create a formal Record of Processing Activities (ROPA) and conduct a Data Protection Impact Assessment (DPIA).
* **Residual Risk:** Medium
* **Owner:** Privacy Officer / Legal Counsel

---

## Top 3 Ranked Risks

1. **RSK-02 (Critical): Unprotected Privileged Accounts** — Lack of MFA on admin accounts creates an immediate, open door for total organizational compromise.
2. **RSK-07 (Critical): Undocumented Customer Personal Data / Privacy Compliance** — Operating without a privacy risk assessment or Record of Processing Activities exposes DesertTech to heavy UAE regulatory penalties under the UAE PDPL.
3. **RSK-06 (Critical): Unpatched Critical Vulnerabilities (>90 Days)** — Leaving critical system vulnerabilities open for months drastically increases the window of opportunity for attackers.

