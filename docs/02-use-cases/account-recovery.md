# Scenario 2: Account Recovery / Password Reset / High‑Value Helpdesk Requests
This scenario describes how Verified ID and Face Check can protect helpdesk workflows from impersonation and social engineering attacks.

## Goal
Prevent social engineering and impersonation during service desk recovery scenarios.

## Functional Steps to Test
1. A user contacts the helpdesk for a high‑risk action:
   - Account recovery  
   - Password reset  
   - MFA re‑registration  
   - Device re‑enrolment
2. The helpdesk workflow initiates identity verification.
3. The user presents their organisation‑issued Verified ID.
4. For high‑risk actions, Face Check is triggered.
5. The user completes live selfie and liveness verification.
6. The workflow receives the verification outcome.
7. Only successful verification allows the helpdesk to proceed.
8. Failed verification routes the request to a controlled fallback process.

## Expected Outcomes
- Identity is validated before recovery actions occur.
- Verification is resistant to social‑engineering attacks.
- Biometric data is never exposed to helpdesk staff.
