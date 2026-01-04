# Conditional Access Policy Set

## Baseline Security Policies

### CA-01 | Require MFA – All Users
- Scope: All users
- Exclusions: Break-glass account
- Control: Require multi-factor authentication

### CA-02 | Block Legacy Authentication
- Scope: All users
- Client apps: Legacy authentication protocols
- Action: Block access

## Privileged Access Protection

### CA-03 | Require MFA – Admin Portals
- Scope: Directory roles
- Applications: Azure Management & Entra Admin portals
- Control: Require MFA

### CA-04 | Admins Require Compliant Device
- Scope: Privileged roles
- Control: Require compliant or hybrid-joined device

## Risk-Based Controls

### CA-05 | Block High-Risk Sign-ins
- Condition: Sign-in risk = High
- Action: Block access

### CA-06 | Require Password Change – High User Risk
- Condition: User risk = High
- Action: Force password reset

## Design Notes
- Break-glass account is excluded from all policies
- Policies are layered to prevent tenant lockout
- Risk-based controls leverage Entra Identity Protection
