# Architecture Overview — Enterprise Zero Trust Identity

## Context
This project implements an identity-first Zero Trust architecture using Microsoft Entra ID (Azure AD) within a single enterprise tenant. The design aligns with Microsoft Zero Trust principles by enforcing explicit verification, least-privilege access, and continuous risk evaluation.

## Objectives
- Eliminate implicit trust based on network or location
- Enforce strong authentication using MFA and Conditional Access
- Secure privileged access using just-in-time elevation
- Ensure recoverability through controlled emergency access
- Provide centralized logging and audit visibility

## Zero Trust Principles Applied
- Identity as the primary security control plane
- Access decisions based on user, device, location, and risk
- Privileged access is time-bound and monitored
- Exceptions are explicit, documented, and audited

## Control Plane Components
- Microsoft Entra ID (Identity Provider)
- Conditional Access (Policy Enforcement)
- Privileged Identity Management (PIM)
- Identity Protection (Risk-Based Detection)
- Entra Sign-in & Audit Logs

## Outcomes
- Reduced attack surface
- Strong separation between standard and privileged access
- Continuous verification for all identities
- Enterprise-grade identity resilience
