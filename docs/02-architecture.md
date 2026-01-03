# Identity and Role Model

## Identity Types

### 1. Bootstrap Identity
- Type: Microsoft Account (External)
- Purpose: Tenant ownership and recovery
- Usage: Not used for daily administration

### 2. Daily Admin Identity
- UPN: goddy.admin@cloud.goddyotuwho.com
- Type: Native Entra ID user
- Security:
  - MFA enforced
  - Privileged roles via PIM
- Purpose: Day-to-day administration

### 3. Break-Glass Identity
- UPN: breakglass@cloud.goddyotuwho.com
- Type: Native Entra ID user
- Security:
  - No MFA
  - Excluded from Conditional Access
- Purpose: Emergency tenant recovery only

### 4. Standard Users
- Employees and contractors
- MFA enforced
- Access governed by Conditional Access

## Role Assignment Strategy
- No permanent Global Administrators
- Admin roles assigned as **Eligible** via PIM
- Time-bound access with justification
