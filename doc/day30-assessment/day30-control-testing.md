# Control Testing Workpaper — DesertTech Solutions
**Company:** DesertTech Solutions  
**Date:** August 2026  
**Scope:** Preliminary Review Findings (Day 30 Assessment)  

---

## Control Test 1: Account Termination

* **Control:** Automated or documented manual account deactivation upon employee termination.
* **Control Objective:** Ensure former employees lose access to corporate systems and data immediately upon departure.
* **Test Procedure:** Sample 5 recently departed employees from HR records and verify whether their Microsoft 365 accounts were disabled within 24 hours of exit.
* **Evidence Requested:** HR termination register and Microsoft 365 Entra ID audit logs showing account status and last login timestamps.
* **Expected Evidence:** Active status marked as "False/Disabled" and immediate termination tickets logged in the IT helpdesk system.
* **Actual Evidence:** 5 former employees still show active M365 accounts with active sessions and recent login activity.
* **Test Result:** Ineffective
* **Finding:** Dormant accounts belonging to former employees remain active in the cloud environment.
* **Risk:** Unauthorized access to cloud environment via dormant accounts (RSK-01).
* **Recommendation:** Immediately disable the 5 active accounts and implement an automated offboarding checklist integrated between HR and IT.

---

## Control Test 2: Multi-Factor Authentication (MFA) for Privileged Accounts

* **Control:** Mandatory Multi-Factor Authentication for all administrative and privileged user accounts.
* **Control Objective:** Prevent unauthorized administrative access resulting from compromised credentials.
* **Test Procedure:** Review the list of all users assigned privileged roles (Global Administrator, Security Administrator) and cross-reference them with active MFA registration policies.
* **Evidence Requested:** Azure AD / Entra ID administrative role assignment report and MFA authentication method registration logs.
* **Expected Evidence:** 100% of privileged accounts enforced with phishing-resistant or standard MFA.
* **Actual Evidence:** 3 privileged accounts lack MFA enforcement, relying solely on passwords.
* **Test Result:** Ineffective
* **Finding:** Administrative accounts are operating without second-factor authentication.
* **Risk:** Compromise of administrative accounts leading to total tenant takeover (RSK-02).
* **Recommendation:** Enforce immediate MFA registration and configure a mandatory Conditional Access policy for all administrative roles.

---

## Control Test 3: Backup Restoration Testing

* **Control:** Periodic testing of system and database backup restoration.
* **Control Objective:** Ensure data integrity and verify that backups can be successfully restored within acceptable Recovery Time Objectives (RTO).
* **Test Procedure:** Inspect backup administration logs and request documentation or test reports of recent backup restoration drills conducted over the past 12 months.
* **Evidence Requested:** Backup schedule configurations, backup success logs, and periodic backup restore test reports/minutes.
* **Expected Evidence:** Documented quarterly backup restoration test results verifying data recovery capability.
* **Actual Evidence:** Automated daily backup jobs are running, but zero evidence or documentation of a recent restore test exists.
* **Test Result:** Partially Effective
* **Finding:** Backups are captured daily, but data restorability has never been verified through testing.
* **Risk:** Permanent data loss or extended operational downtime following a disruptive incident (RSK-04).
* **Recommendation:** Establish and execute a bi-annual backup restoration testing procedure and maintain formal test logs.

