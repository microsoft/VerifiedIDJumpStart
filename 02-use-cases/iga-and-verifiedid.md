# Scenario 4: Access to Sensitive Information / Privilege Escalation (Entra IGA)

## Goal
Ensure strong identity verification before granting access to sensitive systems or privileged roles.

## Functional Steps to Test
1. A user requests sensitive access.
2. The request is routed via Identity Governance (for example, an access package).
3. Verified ID presentation is required.
4. Face Check is enforced for high‑risk access.
5. The user completes Face Check validation.
6. The verification result is recorded.
7. Approvers review the request with verification context.
8. Access is granted only after successful verification and approval.

## Expected Outcomes
- Verified ID is enforced at request time.
- Face Check results are visible to the workflow.
- Access is granted only after successful verification.
