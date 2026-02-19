
# Verified ID Operational Flow for Sensitive Actions

This document describes how Microsoft Entra Verified ID can be used as a reusable identity verification control across onboarding, sensitive access requests, risk-based enforcement, and helpdesk recovery scenarios. The flow demonstrates how a single verification pattern (VID Check Phase) can be invoked at multiple trust boundaries to reduce fraud, impersonation, and social engineering risk.
---

## Overview

This flow illustrates how **Microsoft Entra Verified ID** and **Face Check**
can be embedded into day-to-day identity operations as a **step-up trust control**.

Rather than being a one-time onboarding activity, Verified ID becomes a **repeatable,
policy-driven verification mechanism** that can be invoked whenever confidence
in a user’s identity is required—without storing biometric data or exposing PII.

Organisations evaluating Verified ID can use this as a **starting reference architecture**,
then adapt decision points, policies, and confidence thresholds to match their
own risk appetite and regulatory requirements.

---

## A. Onboard and Issue the Credential

1. A new user joins the organisation and onboarding begins.  
2. The user’s identity is validated according to organisational policy  
   (for example, workforce proofing or government ID proofing where required).  
3. The organisation issues a **Verified ID credential**, which the user receives
   in the **Microsoft Authenticator wallet**.

✅ Outcome: The user now holds a **cryptographically verifiable credential**
that can be reused across multiple trust decisions.

---

## B. Sensitive Access Requested

4. The user requests access to a sensitive application, dataset, or privileged role.  
5. The flow transitions to **X. VID Check Phase**.  
6. The system receives a **match confidence score** from the verification process.  
7. Access is **granted or denied** based on policy thresholds.

✅ Outcome: Sensitive access is protected using **strong identity verification**
instead of static secrets or knowledge-based checks.

---

## C. Risk Is Detected

8. A risk event or unusual activity is detected  
   (for example, anomalous sign-in, high-risk action, or policy trigger).  
9. The flow transitions to **X. VID Check Phase**.  
10. If **Face Check passes**, the action continues.  
11. If it **fails**, the action is blocked and escalated according to policy.

✅ Outcome: Identity confidence is re-established **in real time** before allowing
a risky action to proceed.

---

## D. User Forgets Password (Helpdesk Scenario)

12. The user contacts the helpdesk for password recovery.  
13. The flow transitions to **X. VID Check Phase**.  
14. If verification **passes**, the user is allowed to reset their password
    or complete recovery steps.  
15. If verification **fails**, the user follows an alternate recovery process.

✅ Outcome: Helpdesk impersonation and social engineering risk is significantly reduced.

---

## X. VID Check Phase (Reusable Verification Pattern)

16. The user is prompted to open the **Microsoft Authenticator app**.  
17. The app selects the appropriate **Verified ID credential**.  
18. The user completes the verification request.  
19. The user completes **Face Check** if required.  
20. The system performs **liveness detection** and matches against the enrolled profile.  
21. The system returns **only a confidence score** to the relying system.  
22. The system **discards the selfie and any PII** collected during verification.

✅ Outcome: Strong verification with **privacy-by-design** and **no biometric storage**.

---

## Key Design Principles

- **Reusable trust control** – one verification pattern, many scenarios  
- **Privacy-preserving** – no biometric data retained  
- **Policy-driven** – confidence thresholds aligned to business risk  
- **Phishing-resistant** – removes reliance on knowledge-based verification  

---

## Public References

- Microsoft Entra Verified ID overview  
  https://learn.microsoft.com/entra/verified-id/  

- Face Check for Verified ID  
  https://learn.microsoft.com/entra/verified-id/face-check  

- Microsoft Authenticator  
  https://learn.microsoft.com/entra/identity/authenticator/  

---
