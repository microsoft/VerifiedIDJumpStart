# One‑Page Process Flow

This page provides an end‑to‑end view of how Verified ID and Face Check are used across onboarding, access requests, risk‑based step‑up, and account recovery.

## 1. Onboard and Issue the Credential
1. A new user joins the organisation.
2. Identity is validated according to policy.
3. Verified ID is issued and stored in Microsoft Authenticator.

## 2. Sensitive Access Request with Face Check
4. The user requests sensitive access via governance workflows.
5. The Verified ID check phase begins.
6. The match result determines access approval or denial.

## 3. Risk‑Based Step‑Up Verification
7. Risk signals are detected.
8. Face Check is required again.
9. Successful verification allows continuation.
10. Failure blocks and escalates the action.

## 4. Account Recovery via Helpdesk
11. The user initiates recovery.
12. Verified ID and Face Check are required.
13. Recovery proceeds only after successful verification.

## 5. Verified ID Check Flow
15. Verified ID is presented.
16. The user completes verification in Authenticator.
17. Face Check is applied where higher assurance is required.
18. Only verification outcomes are returned and logged.
