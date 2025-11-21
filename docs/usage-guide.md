---
title: Usage Guide
description: Learn how to use VeriMeZK step-by-step, from scanning documents to verifying proofs.
keywords: [VeriMeZK, usage, guide, flow, identity, verification]
slug: /usage-guide
---

# Usage Guide

This guide walks through the complete VeriMeZK flow, from scanning a document to verifying a proof.

## User Flow

1. **Scan the document** to extract MRZ data.
2. **Verify the face** to confirm liveness and a biometric match.
3. **Select a rule** that defines the attribute to prove (for example, over 18).
4. **Generate the proof** locally on the user's device.
5. **Verify the proof** either on-chain via Midnight or off-chain within your application.

## Example: Over-18 Verification

- The user scans a passport.
- Face verification succeeds.
- The "Over 18" rule is selected.
- A proof is generated locally.
- The proof is verified on-chain for access control.

## Reusability Considerations

- Proofs can be trusted across multiple applications.
- Rules can be tailored to specific compliance or product needs.
