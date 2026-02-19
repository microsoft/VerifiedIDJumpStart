## Relative Priority – Suggested Rollout Order

This section outlines a **recommended phased rollout order** for adopting Microsoft Entra Verified ID and Face Check.  
The prioritisation is based on **risk reduction**, **business impact**, and **implementation effort**, and is intended to help organisations focus first on scenarios that deliver the **fastest and most defensible security value**.

This guidance is **not prescriptive**. It provides a starting point for design workshops, pilots, and production planning, and should be adjusted based on:
- Organisational risk appetite and threat model  
- User personas (employees, contractors, admins, executives)  
- Regulatory and compliance obligations  
- Existing identity, governance, and access controls maturity  

---

### Foundation: Credential Issuance (P0)

**Verified ID issuance is the foundational prerequisite** for all downstream verification scenarios.  
Without a trusted credential issued to users, higher‑assurance verification (including Face Check) cannot be enforced consistently across workflows.

**Why this comes first**
- Establishes a reusable, organisation‑issued credential
- Enables consistent verification across onboarding, recovery, and access scenarios
- Avoids one‑off identity checks that cannot scale or be audited

**Typical focus areas**
- Enable self‑issuance of Verified ID for employees and contractors
- Use **Quick Setup** to accelerate time‑to‑value while planning deeper onboarding integration
- Optionally introduce **government ID pre‑verification** for higher‑risk onboarding populations (e.g. contractors, privileged users)

**Relevant documentation**
- Quick setup of Microsoft Entra Verified ID tenant  
  https://learn.microsoft.com/en-us/entra/verified-id/verifiable-credentials-configure-tenant-quick  
- Advanced Microsoft Entra Verified ID setup  
  https://learn.microsoft.com/en-us/entra/verified-id/verifiable-credentials-configure-tenant  

---

### Highest Value / Fastest Risk Reduction (P1)
#### <ins> Account Recovery / Helpdesk Workflows </ins>

These scenarios represent **real‑world, high‑frequency impersonation risk** and are commonly targeted by social engineering and credential‑based attacks.  
Applying Verified ID and Face Check here typically delivers immediate security uplift with minimal disruption.

**Why it matters**
- Helpdesk recovery is a primary entry point for social engineering attacks
- Password resets, MFA re‑registration, and device recovery are high‑impact actions

**Value delivered**
- Prevents impersonation during recovery
- Ensures biometric data is never exposed to helpdesk staff
- Provides auditable, privacy‑preserving verification

**Documentation**
- Verified helpdesk with Microsoft Entra Verified ID  
  https://learn.microsoft.com/en-us/entra/verified-id/helpdesk-with-verified-id  

#### <ins> Controlled / Administrator Access </ins>

**Why it matters**
- Administrator credentials are high‑value targets
- Remote impersonation of admins has outsized impact

**Value delivered**
- Confirms real administrator presence before sensitive operations
- Strengthens audit and assurance for privileged actions
- Reduces risk of credential theft and replay attacks

#### <ins> High‑Profile User Sensitive Access </ins>

**Why it matters**
- Executives and board members are frequent impersonation targets
- Impact of compromise is disproportionately high

**Value delivered**
- Aligns identity assurance with role criticality
- Applies appropriate verification friction for high‑impact actions
- Produces auditable verification outcomes

---

### Next Wave: Governed Sensitive Access (P2)

Once issuance and high‑risk recovery paths are protected, organisations typically extend Verified ID into **governed access decisions**.

#### <ins> Privilege Escalation via Identity Governance </ins>

**Why it matters**
- Sensitive applications, data sets, and roles require stronger proof than authentication alone
- Approvers benefit from verification context

**Value delivered**
- Enforces Verified ID at access request time
- Integrates Face Check into approval workflows for high‑risk entitlements
- Ensures access is granted only after successful verification and approval

**Documentation**
- Configure Verified ID settings for access packages  
  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-verified-id-settings  

---

### Expansion Scenarios (P3)

These scenarios typically follow once foundational controls and governance integrations are in place.  
They deliver **scale, consistency, and operational efficiency** across broader populations and environments.

#### <ins> Remote Onboarding at Scale </ins>
- Extends high‑assurance onboarding to large frontline or contractor populations
- Reduces reliance on manual or in‑person identity checks
- Improves onboarding speed while maintaining strong assurance

#### <ins> Physical Site Access </ins>
- Validates real person presence before granting site entry
- Supports temporary and time‑bound access
- Avoids exposing biometric data to physical access systems

---

> **Note:** P2 and P3 ordering may vary by organisation.  
> For example, environments with heavy contractor usage may prioritise physical access earlier, while regulated industries may prioritise Identity Governance use cases.

This phased approach helps organisations **start small, reduce risk early, and expand confidently**, while ensuring identity assurance scales
