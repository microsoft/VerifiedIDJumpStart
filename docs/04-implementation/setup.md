# Setup Process

This page outlines the typical setup sequence for enabling Microsoft Entra Verified ID and Face Check.

|#| Step | What You Do | Microsoft Documentation |
|---|-----|------------|------------------------|
|1| Configure Verified ID | Enable Verified ID using quick or advanced setup | [Quick setup](https://learn.microsoft.com/en-us/entra/verified-id/verifiable-credentials-configure-tenant-quick) / [Advanced setup](https://learn.microsoft.com/en-us/entra/verified-id/verifiable-credentials-configure-tenant) |
|2| Define issuance model | Decide which credential is issued and how users obtain it | Included in quick setup |
|3| Enable Face Check | Enable Face Check add‑on and link Azure subscription | [Using Face Check](https://learn.microsoft.com/en-us/entra/verified-id/using-facecheck) |
|4| Integrate workflows | Connect verification to helpdesk and access portals | [Verified helpdesk pattern](https://learn.microsoft.com/en-us/entra/verified-id/helpdesk-with-verified-id) |
|5| Identity Governance | Require Verified ID in access packages | [Configure Verified ID](https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-verified-id-settings) |
|6| Risk triggers (in development) | TBA | TBA |
| Fallback paths | Define manual or alternate processes for cases when employee / contractor 1) cannot be onboarded to verified id process, or 2) cannot complete verification using FaceCheck | As per organisation policy |
