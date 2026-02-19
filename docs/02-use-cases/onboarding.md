# Scenario 1: Remote User Onboarding (Frontline / Contractor / Remote Joiner)
This scenario describes how Verified ID can be used during onboarding to ensure the individual joining the organisation is legitimate before they get access to organisation resource or facilities.

## Goal
Verify that the person onboarding is legitimate before issuing an organisation‑trusted credential that will later be used in high‑risk scenarios.

## Functional Steps to Test
1. A new frontline worker or contractor joins the organisation.
2. Onboarding activities are completed:
   - User account creation  
   - Initial permissions assignment  
   - MFA registration  
   - Device management or compliance checks
3. Identity proofing is completed according to organisational policy (for example, government ID verification via an IDV provider).
4. The organisation issues a Verified ID credential.
5. The user receives the credential in the Microsoft Authenticator wallet.
6. The user successfully presents the credential back to the organisation.

## Expected Outcomes
- Verified ID issuance completes successfully.
- The user can present the credential from their device.
- The credential can later be used in Face Check verification flows.
