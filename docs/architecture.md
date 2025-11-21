---
title: Architecture Overview
description: Understand the modular, privacy-first architecture of VeriMeZK and how its components interact.
keywords: [VeriMeZK, architecture, design, modules, privacy, client-side, ZK]
slug: /architecture
---

# Architecture Overview

VeriMeZK is a **modular, client-side toolkit** for privacy-preserving identity verification based on zero-knowledge proofs.

## Core Components

- **Document scanner** extracts MRZ data from passports and identity cards.
- **Face verifier** performs liveness detection and biometric matching.
- **Proof engine** generates ZKPs according to the selected rules.
- **Verifier** validates proofs on-chain (via Midnight) or off-chain.
- **UI layer** provides reference interfaces and SDK hooks.

## Data Flow

1. A document is scanned and the MRZ data is extracted.
2. Face verification confirms liveness and biometric match.
3. The user or integrator selects the rule to be proven.
4. A zero-knowledge proof is generated locally.
5. The proof is verified and a result is returned to the application.

:::tip
**All processing remains on the user's device.** No identity data is transmitted to external services.
:::

## Privacy by Design

- No backend services are required.
- Identity data is never stored.
- Third-party APIs are not involved in the verification flow.
- All logic executes within the browser environment.

## Extensibility

- Add new rules with [Custom Checks](./features/custom-checks.md).
- Integrate the workflow into applications using the [SDK](./api/sdk-overview.md).
