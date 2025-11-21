---
title: Midnight Blockchain
description: Learn how the Midnight blockchain enables private, on-chain verification of identity proofs in VeriMeZK.
keywords:
  [Midnight, blockchain, privacy, smart contracts, zero-knowledge, identity]
slug: /concepts/midnight-blockchain
---

# Midnight Blockchain

**Midnight** is a privacy-first blockchain that supports confidential smart contracts and zero-knowledge proof verification. VeriMeZK uses Midnight to deliver on-chain identity verification without exposing personal data.

## Why Midnight?

Midnight is built for:

- Confidential smart contracts
- Zero-knowledge-friendly architecture
- Decentralised identity use cases
- Regulatory compliance without data leakage

## How VeriMeZK Uses Midnight

1. A user generates a zero-knowledge proof locally.
2. The proof is submitted to a smart contract on Midnight.
3. The contract verifies the proof against the requested rule.
4. The result can be referenced within a dApp or stored for audit trails.

:::tip
A DAO running on Midnight can require an "over 18" proof to vote without ever receiving the voter's age.
:::

## Privacy by Design

- No personal data is stored on-chain.
- Document and biometric data remain on the user's device.
- Only the proof artifact and associated rule are included in the transaction.

## Integration Requirements

- Wallet connection compatible with Midnight
- Smart contract containing the desired verification logic
- Optional front-end dApp powered by the VeriMeZK SDK

## Related Topics

- [Midnight Verification](../features/midnight-verification.md)
- [Architecture Overview](../architecture.md)
