# Privileged Identity Management (PIM) and Admin Hardening

## Objectives
- Remove standing administrative privileges
- Enforce least-privilege access through just-in-time elevation
- Improve traceability of administrative actions

## Configuration
- Global Administrator assigned as Eligible
- Role activation requires:
  - MFA
  - Business justification
  - Time-bound duration (1–4 hours)

## Benefits
- Reduced administrative blast radius
- Clear separation between standard and privileged activity
- Full audit trail for all role activations
