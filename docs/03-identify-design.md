# Conditional Access Policy Set

## Baseline Policies

### CA-01 | Require MFA – All Users
- Scope: All users
- Exclusions: Break-glass account
- Controls: Require MFA

### CA-02 | Block Legacy Authentication
- Scope: All users
- Client apps: Legacy protocols
- Action: Block access

## Privileged Access Policies

### CA-03 | Require MFA – Admin Portals
- Scope: Directory roles
- Apps: Azure Management, Entra Admin Center
- Controls: Require MFA

### CA-04 | Admins Require Compliant Device
- Scope: Privileged roles
- Controls: Require compliant device

## Risk-Based Policies

### CA-05 | Block High-Risk Sign-ins
- Condition: Sign-in risk = High
- Action: Block access

### CA-06 | Require Password Change – High User Risk
- Condition: User risk = High
- Action: Require password change

## Design Notes
- All policies explicitly exclude the break-glass account
- Policies are layered to avoid lockout
- Risk-based controls rely on Identity Protection signals
