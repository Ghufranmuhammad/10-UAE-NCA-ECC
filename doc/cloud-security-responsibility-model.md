# Cloud Security Shared Responsibility Model

## Introduction

The shared responsibility model explains how security responsibilities are divided between a cloud service provider and the customer.

The exact division depends on the cloud service model. In general, the provider is responsible for security **of** the underlying cloud infrastructure, while the customer remains responsible for security **in** the cloud.

---

## Responsibility Matrix

| Area | Cloud Provider | Customer |
|---|---|---|
| Physical Data Center | Responsible | — |
| Physical Infrastructure | Responsible | — |
| Hypervisor / Core Cloud Platform | Responsible | — |
| User Access | — | Responsible |
| Identity and MFA | — | Responsible |
| Data Classification | — | Responsible |
| Customer Data | — | Responsible |
| Application Configuration | Shared / Depends on Service | Responsible where applicable |
| Operating System | Shared / Depends on Service | Responsible in IaaS |
| Network Controls | Shared | Responsible for customer-side configuration |
| Logging | Shared | Responsible for reviewing customer-side logs |
| Backup | Shared / Depends on Service | Customer responsible for required backup strategy |
| Incident Response | Shared | Shared |
| Vulnerability Management | Shared | Customer responsible for customer-managed components |
| Security Configuration | Shared | Customer responsible for customer-side settings |

---

# Why This Matters to a GRC Analyst

A GRC Analyst needs to understand the shared responsibility model because moving systems to the cloud does not transfer all security responsibilities to the cloud provider.

For example, a cloud provider may secure the physical data center, but DesertTech could still be responsible for:

- User access
- MFA
- Data classification
- Customer-side configuration
- Permissions
- Logging and monitoring
- Backup requirements
- Incident response activities

A GRC Analyst should therefore verify:

1. Which responsibilities belong to the provider?
2. Which responsibilities belong to DesertTech?
3. Which controls are shared?
4. What contractual commitments exist?
5. What evidence does the provider provide?
6. What evidence must DesertTech maintain itself?

Understanding this prevents control gaps caused by the assumption that "the cloud provider handles security."

---

# DesertTech Example

DesertTech uses a fictional cloud provider, DesertCloud Services, to host critical applications.

The provider is responsible for the physical data center and underlying infrastructure.

DesertTech remains responsible for user access, MFA, data classification, customer-side configurations, monitoring, and its own security processes.

The GRC team documents these responsibilities and verifies that evidence exists for both provider and customer responsibilities.
