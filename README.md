# Project 01 — Enterprise Zero Trust Identity Architecture (Microsoft Entra ID)

## Overview
This repository demonstrates an enterprise-grade Zero Trust Identity architecture implemented in Microsoft Entra ID (Azure AD). The solution enforces **least privilege**, **continuous verification**, and **risk-based access** using Conditional Access, MFA, PIM, and Identity Protection—aligned to Microsoft Zero Trust principles.

## Goals
- Implement identity-first Zero Trust controls (MFA, Conditional Access, Identity Protection)
- Protect privileged access using PIM and role separation
- Provide audit-ready logging and monitoring (sign-in logs, audit logs)
- Document policy decisions, test scenarios, and evidence

## Architecture
![Zero Trust Identity Architecture](architecture/diagrams/zero-trust-identity-architecture.png)

## Key Capabilities Implemented
- Conditional Access policy set (baseline + privileged access)
- Legacy authentication blocked
- Admin access hardened (PIM, MFA, compliant device requirements)
- Break-glass recovery design (excluded from CA, monitored)
- Sign-in log monitoring and auditability

## Repository Guide
- `docs/` — architecture overview, identity model, monitoring, tests
- `policies/` — Conditional Access + PIM configurations (documented)
- `architecture/` — diagram + decision records (ADRs)
- `evidence/` — screenshots and implementation notes

## Test Scenarios (Examples)
- Normal user sign-in requires MFA
- Legacy auth attempts are blocked
- Admin role activation requires MFA + justification (PIM)
- High-risk sign-ins trigger enforcement actions
- Break-glass account access remains available (emergency only)

## Notes
This is a portfolio implementation for demonstrating enterprise security architecture patterns. It is designed to be defensible in interviews with clear rationale, controls, and evidence.
