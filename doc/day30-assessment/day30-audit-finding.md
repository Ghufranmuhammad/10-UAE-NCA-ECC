# Formal Audit Finding — DesertTech Solutions
**Company:** DesertTech Solutions  
**Date:** August 2026  
**Scope:** Preliminary Review Findings (Day 30 Assessment)  

---

## Finding Title: 
Absence of Multi-Factor Authentication (MFA) on Privileged Administrator Accounts

### Observation:
During our preliminary access review of the Microsoft 365 and Azure cloud environment, it was identified that three (3) privileged administrator accounts are configured without Multi-Factor Authentication (MFA) enforcement. These accounts rely solely on standard password-based authentication.

### Requirement/Expectation:
Industry security standards (such as ISO 27001 Control A.9.4.2 and NCA ECC Control IAM-01-01) and internal security guidelines require all privileged and administrative accounts to be protected with mandatory, robust multi-factor authentication to prevent unauthorized credential-based access.

### Evidence:
* Azure AD / Entra ID administrative role assignment export listing active Global and Security Administrators.
* Conditional Access policy configuration screen showing no active MFA enforcement policy applied to the identified admin accounts.

### Risk:
Compromise of administrative accounts leading to total tenant takeover, data exfiltration, system manipulation, and complete operational disruption (Risk ID: RSK-02).

### Severity:
Critical

### Root Cause:
Exclusion or misconfiguration during the initial setup of cloud administrative roles, combined with a lack of automated enforcement policies across privileged groups.

### Recommendation:
1. Immediately enforce mandatory MFA for all 3 un-protected privileged accounts.
2. Implement a strict Azure AD Conditional Access policy that blocks admin sign-ins unless multiple authentication factors are satisfied.
3. Conduct a comprehensive review of all other privileged group memberships to ensure full coverage.

### Management Action:
Management agrees with the finding and has scheduled the enforcement of Conditional Access policies for all administrators.

### Owner:
IT Security Lead

### Target Date:
August 25, 2026

