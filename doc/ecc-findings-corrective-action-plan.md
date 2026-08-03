# DesertTech Solutions – ECC Findings & Corrective Action Plan

## Finding NC-001

**Finding ID:** NC-001

**Control Area:** Vulnerability Management

**Observation:** Several critical vulnerabilities exceeded the defined remediation timeline.

**Expected Requirement:** Critical vulnerabilities should be identified, prioritized, and remediated within defined organizational timelines.

**Evidence:** Monthly Vulnerability Scan Report.

**Risk:** Attackers may exploit known vulnerabilities to compromise systems.

**Severity:** High

**Root Cause:** Remediation tracking and escalation are not sufficiently automated.

**Recommendation:** Implement automated vulnerability tracking and escalation for overdue critical findings.

**Management Action:** Security Team will implement automated remediation tracking and establish escalation procedures.

**Owner:** Security Manager

**Due Date:** 2026-09-15

**Status:** Open

---

## Finding NC-002

**Finding ID:** NC-002

**Control Area:** Patch Management

**Observation:** Several critical servers were overdue for security patches.

**Expected Requirement:** Security patches should be applied according to defined timelines.

**Evidence:** Patch Compliance Report.

**Risk:** Unpatched systems may be exploited by attackers.

**Severity:** High

**Root Cause:** Manual patch tracking and inconsistent remediation follow-up.

**Recommendation:** Implement automated patch compliance monitoring.

**Management Action:** Infrastructure Team will establish automated patch reporting and escalation.

**Owner:** Infrastructure Manager

**Due Date:** 2026-09-20

**Status:** Open

---

## Finding NC-003

**Finding ID:** NC-003

**Control Area:** Backup Management

**Observation:** One critical system did not have recent backup restoration testing evidence.

**Expected Requirement:** Critical backups should be periodically tested to confirm recoverability.

**Evidence:** Backup Test Report.

**Risk:** DesertTech may be unable to recover critical information following a system failure or cyberattack.

**Severity:** High

**Root Cause:** Backup restoration testing does not cover every critical system consistently.

**Recommendation:** Establish quarterly restore testing for all critical systems.

**Management Action:** IT Team will expand the restoration testing schedule.

**Owner:** IT Manager

**Due Date:** 2026-09-30

**Status:** Open

---

## Finding NC-004

**Finding ID:** NC-004

**Control Area:** Business Continuity

**Observation:** The latest BCP exercise did not cover all critical business services.

**Expected Requirement:** Business continuity testing should validate recovery capabilities for critical services.

**Evidence:** BCP Test Report.

**Risk:** DesertTech may experience extended disruption if an untested critical service fails.

**Severity:** Medium

**Root Cause:** BCP testing scope was not mapped against the complete critical service inventory.

**Recommendation:** Update the BCP testing scope and include all critical services.

**Management Action:** GRC and IT Teams will update the annual BCP exercise plan.

**Owner:** GRC Manager

**Due Date:** 2026-10-15

**Status:** Open

---

## Finding NC-005

**Finding ID:** NC-005

**Control Area:** Third-Party Risk Management

**Observation:** One Critical vendor security assessment was overdue.

**Expected Requirement:** Critical suppliers should be periodically assessed according to their risk classification.

**Evidence:** Vendor Risk Register.

**Risk:** A change in the supplier's security posture may remain unidentified.

**Severity:** High

**Root Cause:** Vendor review dates are tracked manually.

**Recommendation:** Implement automated reminders and escalation for overdue vendor assessments.

**Management Action:** GRC Team will complete the overdue assessment and establish automated review reminders.

**Owner:** GRC Manager

**Due Date:** 2026-09-10

**Status:** Open

---

# Findings Summary

| Finding | Severity | Owner | Corrective Action | Deadline |
|---|---|---|---|---|
| NC-001 – Vulnerability Management | High | Security Manager | Automate vulnerability tracking and escalation | 2026-09-15 |
| NC-002 – Patch Management | High | Infrastructure Manager | Improve automated patch compliance monitoring | 2026-09-20 |
| NC-003 – Backup Testing | High | IT Manager | Test restoration of all critical systems | 2026-09-30 |
| NC-004 – Business Continuity | Medium | GRC Manager | Expand BCP exercise scope | 2026-10-15 |
| NC-005 – Third-Party Risk | High | GRC Manager | Complete vendor assessment and automate reminders | 2026-09-10 |
