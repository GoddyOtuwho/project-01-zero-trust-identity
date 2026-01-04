# Break-Glass and Emergency Access

## Purpose
The break-glass account provides guaranteed tenant access during critical incidents such as:
- MFA service outage
- Conditional Access misconfiguration
- Privileged Identity Management failure
- Identity control-plane disruptions

## Account Characteristics
- Native Entra ID user
- Global Administrator role
- MFA intentionally disabled
- Excluded from all Conditional Access policies
- Long, complex, randomly generated password

## Governance and Usage
- Used only for emergency recovery
- Credentials stored securely offline
- Sign-in activity continuously monitored
- Periodic access validation performed

## Security Rationale
Break-glass access represents a documented Zero Trust exception that balances strong enforcement with operational resilience and recoverability.
