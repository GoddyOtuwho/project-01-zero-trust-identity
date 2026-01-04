# CA-04 | Admins Require Compliant Device

## Objective
Ensure privileged access occurs only from trusted devices.

## Scope
- Users: Directory roles
- Exclusions: breakglass@cloud.goddyotuwho.com

## Conditions
- Device state: Require compliant or hybrid Azure AD joined device

## Grant Controls
- Require device to be marked as compliant

## Rationale
Restricting admin access to trusted devices reduces the risk of credential theft and session hijacking.
