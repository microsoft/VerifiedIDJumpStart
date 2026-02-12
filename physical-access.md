# Scenario 3: Validate Physical Site Access (Employee / Contractor / Visitor)

## Goal
Confirm that the correct individual is physically present before granting controlled site access.

## Functional Steps to Test
1. The individual arrives at the physical site.
2. Access validation is initiated by reception or security.
3. The individual scans a QR code to launch verification on their mobile device.
4. The Verified ID credential is presented.
5. Face Check is required:
   - Live selfie capture  
   - Liveness detection  
   - Facial match against the Verified ID photo
6. The front desk system receives a pass/fail result.
7. Physical access is granted for a defined time window.
8. Access expires automatically.

## Expected Outcomes
- Live human presence is validated.
- Biometric images are not exposed to onsite systems.
- Failed verification prevents access and triggers alternate procedures.
