# CA-05 | Block High-Risk Sign-ins

## Objective
Deny access when Entra Identity Protection detects high sign-in risk.

## Scope
- Users: All users
- Exclusions: breakglass@cloud.goddyotuwho.com

## Conditions
- Sign-in risk: High

## Grant Controls
- Block access

## Rationale
High-risk sign-ins indicate likely compromise and must be stopped immediately.
