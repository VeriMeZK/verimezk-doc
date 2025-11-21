---
title: Zero-Knowledge Proofs
description: Understand the fundamentals of zero-knowledge proofs and how VeriMeZK uses them for private identity verification.
keywords:
  [zero-knowledge, zk, zk-proof, privacy, cryptography, identity verification]
slug: /concepts/zk-proofs
---

# Zero-Knowledge Proofs (ZKPs)

Zero-knowledge proofs are the cryptographic foundation of VeriMeZK. They let users **prove that a statement is true without revealing the underlying data**.

## What Is a ZKP?

A zero-knowledge proof allows one party (the prover) to convince another party (the verifier) that a statement is correct, while revealing no additional information beyond the validity of the statement.

## Real-World Analogy

Imagine proving you are over 18 without showing your ID. A ZKP enables exactly that experience: the verifier gains confidence in the claim, but sees no personal details.

:::tip
For example, you can prove "I am over 18" without exposing your birthdate.
:::

## Why ZKPs Matter for Identity

- **Privacy:** Personal data is never exposed.
- **Security:** Sensitive information is not transmitted or stored.
- **Compliance:** Supports KYC/AML checks without data retention.
- **User control:** Individuals choose what to disclose and when.

## Proof Types in VeriMeZK

- Age verification (for example, over 18 or over 21)
- Nationality confirmation (for example, an EU citizen)
- Document validity (not expired or revoked)
- Biometric match (face matches the document image)

## How It Works in VeriMeZK

1. Document and face data are captured locally.
2. The user selects a rule to prove (for example, "is an adult").
3. A ZK proof is generated in the browser.
4. The proof is shared with a verifier on-chain or off-chain.

## Learn More

- [Proof Generation](../features/proof-generation.md)
- [Custom Checks](../features/custom-checks.md)
