# Setup Process

This page outlines the typical setup sequence for enabling Microsoft Entra Verified ID and Face Check.

| Step | What You Do | Microsoft Documentation |
|-----|------------|------------------------|
| Configure Verified ID | Enable Verified ID using quick or advanced setup | [Quick setup](https://learn.microsoft.com/en-us/entra/verified-id/verifiable-credentials-configure-tenant-quick) / [Advanced setup](https://learn.microsoft.com/en-us/entra/verified-id/verifiable-credentials-configure-tenant) |
| Define issuance model | Decide which credential is issued and how users obtain it | Included in quick setup |
| Enable Face Check | Enable Face Check add‑on and link Azure subscription | [Using Face Check](https://learn.microsoft.com/en-us/entra/verified-id/using-facecheck) |
| Integrate workflows | Connect verification to helpdesk and access portals | [Verified helpdesk pattern](https://learn.microsoft.com/en-us/entra/verified-id/helpdesk-with-verified-id) |
| Identity Governance | Require Verified ID in access packages | [Configure Verified ID](https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-verified-id-settings) |
| Risk triggers | Define when step‑up verification is required | [Authentication strengths](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-strengths) |
| Fallback paths | Define manual or alternate processes | Customer policy |
