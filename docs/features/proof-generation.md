---
title: Proof Generation
description: Learn how VeriMeZK generates zero-knowledge proofs locally to validate identity attributes without revealing personal data.
keywords: [VeriMeZK, proof generation, zero-knowledge, zk, identity, privacy]
slug: /features/proof-generation
---

# Proof Generation

VeriMeZK enables users to generate **zero-knowledge proofs (ZKPs)** that confirm specific identity attributes without exposing the underlying data.

## What Is a ZK Proof?

A zero-knowledge proof lets someone show that a statement, such as "I am over 18," is true without disclosing supporting personal information like a birthdate.

## How VeriMeZK Generates Proofs

1. The user selects a rule (for example, "Over 18" or "Is an EU citizen").
2. The application draws on the scanned document data and face-match result.
3. A ZK proof is computed locally in the browser.
4. The proof is formatted for on-chain or off-chain verification.

:::note
No personal data leaves the device. Only the proof and the associated rule are shared.
:::

## Example

Consider a user who wants to prove they are over 18:

- The app reads the birthdate from the scanned document.
- A ZK proof is computed to confirm the user meets the age requirement.
- The proof can be verified, yet the exact birthdate remains private.

## Output Format

Each proof includes:

- The selected rule
- A cryptographic commitment
- A validity flag
- Optional metadata such as timestamp or session identifier

## Next Step

After generating a proof, proceed to [Midnight verification](./midnight-verification.md) or reuse the proof in an off-chain flow.
