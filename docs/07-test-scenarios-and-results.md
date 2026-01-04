# Test Scenarios and Validation Results

## Scenario 1 — Standard User Sign-in
- Expected: MFA challenge
- Result: Access granted after successful MFA

## Scenario 2 — Legacy Authentication Attempt
- Expected: Access blocked
- Result: Sign-in denied

## Scenario 3 — Privileged Role Activation
- Expected: PIM activation with MFA and justification
- Result: Time-bound admin access granted

## Scenario 4 — High-Risk Sign-in
- Expected: Access blocked or password reset enforced
- Result: Risk-based control triggered

## Scenario 5 — Break-Glass Access
- Expected: Emergency access available
- Result: Successful sign-in without CA enforcement
