# Architecture Overview — Enterprise Zero Trust Identity

## Context
This project implements an identity-first Zero Trust architecture using Microsoft Entra ID (Azure AD) in a single enterprise tenant. The design follows Microsoft Zero Trust principles: explicit verification, least privilege access, and continuous risk evaluation.

## Goals
- Eliminate implicit trust based on network location
- Enforce strong authentication using MFA and Conditional Access
- Protect privileged access with Just-In-Time (JIT) elevation
- Enable recoverability through controlled emergency access
- Provide audit-ready logging and visibility

## Core Principles Applied
- Identity is the new control plane
- All access is verified using signals (user, device, location, risk)
- Privileged access is time-bound and monitored
- Exceptions are explicit, documented, and monitored

## Control Plane Components
- Microsoft Entra ID (Identity provider)
- Conditional Access (Policy enforcement)
- Privileged Identity Management (PIM)
- Identity Protection (Risk detection)
- Azure Monitor & Sign-in Logs (Telemetry)

## Outcomes
- Reduced attack surface
- Strong admin isolation
- Policy-driven access decisions
- Recoverable, enterprise-grade identity posture
